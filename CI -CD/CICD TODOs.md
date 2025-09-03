#cicd
- Sentry
	- [x] Configure alerts (hopefully noisier than now) to be in the `#sentry-alerts` channel
	- [ ] Configure all applications to go to their respective projects (using the DSN)
	- [ ] Ensure MDC working correctly in CRUD - can use [Context Tags](https://docs.sentry.io/platforms/java/guides/logback/usage/advanced-usage/) for fun - tehre's a [linear tix for this](https://linear.app/coverdash/issue/WEB-3123/investigate-sentry-stuff)
	- [x] set up gitlab integration
- Gitlab
	- [x] Force squash and (hopefully) only fast-forward merges (in quoting engine first)
		- [x] If ff merges, make sure to update the commit message(s)
		- [x] [Changelogs automation](https://claude.ai/share/4a1cf72c-89d6-460c-9405-33fae675e27a) would be required for us to sqaush everything
			- [x] We can add some sort of connection to Linear to create links, but just having the PR titles should be fine for now
			- [x] Auto create releases from tags

## Changelogs
## 1. Create `.gitlab/changelog_config.yml`

yaml

```yaml
---
date_format: '%Y-%m-%d'
template: |
  ## Release {{version}} - {{date}}
  
  {{#each categories}}
  ### {{title}}
  
  {{#each entries}}
  - {{title}} {{#if merge_request}}([!{{merge_request.iid}}]({{merge_request.web_url}})){{/if}}
  {{/each}}
  
  {{/each}}

categories:
  - title: "🚨 Critical Issues"
    rules:
      - if: $labels =~ /critical/
  - title: "🐛 Bug Fixes"
    rules:
      - if: $labels =~ /bug/
  - title: "✨ Enhancements"
    rules:
      - if: $labels =~ /enhancement/
  - title: "📚 Documentation"
    rules:
      - if: $labels =~ /documentation/
  - title: "💡 Suggestions"
    rules:
      - if: $labels =~ /suggestion/
  - title: "🔧 Support & Maintenance"
    rules:
      - if: $labels =~ /support/
  - title: "🔄 Other Changes"
    rules:
      - if: $labels !~ /critical|bug|enhancement|documentation|suggestion|support|release|discussion|confirmed/
```

## 2. Your Updated CI

yaml

```yaml
tag:
  stage: tag
  when: manual
  image: ${CI_DEPENDENCY_PROXY_DIRECT_GROUP_IMAGE_PREFIX}/alpine:latest
  script:
    - apk add --no-cache git curl jq
    - git fetch --tags --unshallow
    
    # Your existing tag logic...
    - echo "🔍 Finding latest semantic version tag..."
    - LATEST_TAG=$(git tag -l | grep -E '[0-9]+\.[0-9]+\.[0-9]+$' | sort -V | tail -n 1)
    - >
      if [ -z "$LATEST_TAG" ]; then
        echo "ℹ️ No tag found, using default 1.0.0";
        MAJOR=1; MINOR=0; PATCH=0;
      else
        echo "ℹ️ Found tag: $LATEST_TAG";
        VERSION=$(echo "$LATEST_TAG" | grep -oE '[0-9]+\.[0-9]+\.[0-9]+');
        MAJOR=$(echo "$VERSION" | cut -d. -f1);
        MINOR=$(echo "$VERSION" | cut -d. -f2);
        PATCH=$(echo "$VERSION" | cut -d. -f3);
        PATCH=$((PATCH + 1));
        if [ "$PATCH" -gt 9 ]; then PATCH=0; MINOR=$((MINOR + 1)); fi;
        if [ "$MINOR" -gt 9 ]; then MINOR=0; MAJOR=$((MAJOR + 1)); fi;
      fi
    - TAG_NAME="v$MAJOR.$MINOR.$PATCH"
    - echo "🏷️ New tag: $TAG_NAME"
    
    # Create tag
    - git config --global user.email "ci@gitlab.com"
    - git config --global user.name "GitLab CI"
    - git tag -a "$TAG_NAME" -m "Release $TAG_NAME"
    - git push "https://oauth2:${GITLAB_TOKEN}@gitlab.com/${CI_PROJECT_PATH}.git" "$TAG_NAME"
    
    # Generate changelog using GitLab API
    - echo "📝 Generating changelog for $TAG_NAME"
    - |
      if [ -n "$LATEST_TAG" ]; then
        echo "📊 Generating changelog from $LATEST_TAG to $TAG_NAME"
        curl -H "PRIVATE-TOKEN: $GITLAB_TOKEN" \
          "$CI_API_V4_URL/projects/$CI_PROJECT_ID/repository/changelog?version=$TAG_NAME&from=$LATEST_TAG&to=$TAG_NAME" \
          | jq -r .notes > release_notes.md
      else
        echo "📊 Generating changelog for first release"
        curl -H "PRIVATE-TOKEN: $GITLAB_TOKEN" \
          "$CI_API_V4_URL/projects/$CI_PROJECT_ID/repository/changelog?version=$TAG_NAME" \
          | jq -r .notes > release_notes.md
      fi
    
    - echo "📋 Generated changelog:"
    - cat release_notes.md
    
  artifacts:
    paths:
      - release_notes.md
    expire_in: 1 week
  only:
    - release_prod

create_release:
  stage: deploy_PROD
  image: registry.gitlab.com/gitlab-org/release-cli:latest
  needs:
    - job: tag
      artifacts: true
  script:
    - echo "🚀 Creating GitLab release for $CI_COMMIT_TAG"
    - echo "📋 Release notes content:"
    - cat release_notes.md
  release:
    name: 'Release $CI_COMMIT_TAG'
    description: release_notes.md
    tag_name: '$CI_COMMIT_TAG'
    ref: '$CI_COMMIT_SHA'
  rules:
    - if: '$CI_COMMIT_TAG =~ /^v?\d+\.\d+\.\d+$/'
```

## 3. Example Release Notes Output

With your labels, the generated release notes will look like:

markdown

```markdown
## Release v2.1.0 - 2025-07-17

### 🚨 Critical Issues
- Fix authentication timeout causing user lockouts ([!45](https://gitlab.com/merge_requests/45))

### 🐛 Bug Fixes
- Resolve dashboard loading performance issue ([!42](https://gitlab.com/merge_requests/42))
- Fix quote calculation rounding errors ([!43](https://gitlab.com/merge_requests/43))

### ✨ Enhancements
- Add bulk quote processing feature ([!41](https://gitlab.com/merge_requests/41))
- Improve user interface responsiveness ([!44](https://gitlab.com/merge_requests/44))

### 📚 Documentation
- Update API documentation for new endpoints ([!46](https://gitlab.com/merge_requests/46))

### 🔧 Support & Maintenance
- Update dependencies to latest versions ([!47](https://gitlab.com/merge_requests/47))
```

## 4. Team Usage

Now your team just needs to:

1. **Add appropriate labels** to merge requests (bug, enhancement, critical, etc.)
2. **Write clear MR titles** (these become the line items in release notes)
3. **The CI automatically generates** organized release notes based on the labels

## 5. Test It

Add this manual test job to verify it works:

yaml

```yaml
test_changelog:
  stage: build
  image: alpine:latest
  script:
    - apk add curl jq
    - echo "🧪 Testing changelog generation..."
    - |
      curl -H "PRIVATE-TOKEN: $GITLAB_TOKEN" \
        "$CI_API_V4_URL/projects/$CI_PROJECT_ID/repository/changelog?version=test-1.0.0&from=HEAD~10&to=HEAD" \
        | jq -r .notes || echo "No changelog data found - make sure you have labeled MRs"
  rules:
    - when: manual
```

This setup will automatically categorize your release notes based on your existing labels, making it easy to see what types of changes are in each release!