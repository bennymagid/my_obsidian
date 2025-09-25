#selfReview
- Desgined and implemented a javascript playwright script taht navigates carrier login pages to download relevant customer documents after a policy is bound. 
- Improvements to CI/CD
	- No longer need to manually (and dangerously) [allow AWS connections](https://linear.app/coverdash/issue/WEB-997/fix-having-to-add-a-new-temp-security-rule-to-aws-every-time-i-want-to) to our gitlab instance on every release - automated whitelist -- [[🚀 Changes to Release]]
	- [Linter](https://www.notion.so/coverdash/How-to-Set-up-Spotless-Palantir-Linter-in-IntelliJ-23b7c7fc5b0d80469685c18a945d528c?source=copy_link) introduced WEB-3175
	- Release Notes automated with squashing and tagging automation (see below info)
	- Automated deployments
	- Consolidated Ci components library in gitlab
- Presented CNA integration carrier integration [here](https://docs.google.com/presentation/d/1k6I76hS72zeeWrejvt7lrzy6Gqw7UM_gnG_5T806_jg/edit)
- Introduced better practices with [[🏴󠁧󠁢󠁳󠁣󠁴󠁿 Lombok]] to save boilerplate
- Introduced PreHandle usage for more reusable and safer user validation
- Introduced a unified AWS Uploader that will hopefully reduce repeated (and unchecked) code interfacing with S3
- Kudos
	- Feb 11 2025: Kudos 1-month in from Perry for writing clear tickets for FE
	- Feb 11: Kudos from Avery for crushing it in only a month and it feeling like I've been here for 5 months
- Projects
	- Led [major project](https://linear.app/coverdash/issue/WEB-2580/add-csv-importer-for-accounting) early on which involved design and has enabled faster Accountant turnaround and EOM
	- Owned the changes for AE reorg - AEs for different campaigns, Core -> Growth Team transfers
		- Warm Transfer Dashboard has helped see 2x warm transfers from Feb 2024 -> March 2025
- Testing finally (at least some times) [[🍬 Testing Suite]]
- [Documentation](https://www.notion.so/coverdash/How-to-fix-DB-access-issues-18c7c7fc5b0d80a69ca9ce5659dae973?pvs=4) for new hires(!)
- Elected to lead best practices meeting(s)
	- March 11, 2025
		- https://www.notion.so/coverdash/Dev-Den-Backend-Practices-Recap-1ac7c7fc5b0d8078a3dafd1f50cbcc25?pvs=4

- Plans
	- Clearly documented tickets and plans 
		- [AWS migration](https://linear.app/coverdash/issue/WEB-2588/upgrade-aws-s3-sdk-from-v1-v2) 
		- [User validation](https://linear.app/coverdash/issue/WEB-2595/deprecate-validationhelper) -- [[🔑 User Auth]]
		- [enums for PolicyDirection](https://linear.app/coverdash/issue/WEB-2590/replace-hardcoded-string-in-policytransaction-and)
		- Reusable AWS component in `common` - use it and deprecate other bespoke uses
		- More testing finally [[🍬 Testing Suite]]
	- Dependencies(!!)

More CI/CD improvements
Notes I wrote up for the team - gonna let my changes in quoting engine sit for a bit but this would be the flowJust a heads-up for Quoting Engine (piloting CI-CD for the rest of the repos) 

1. I've enforced squashing for branches and fast-forward merges only. You as a MR-author are responsible for ensuring your MR is up to date with its target branch (I can help show you how to rebase / merge easily in the UI if need be)
2. Release Notes
    1. Releases are automatically made after you `tag` something in release_prod
    2. Please also ensure your linear ticket is in the title of the MR as this will make it easier to use the release notes
    3. Please use the Gitlab `label` to help sort your MRs in the release notes or else it will end up in the `Commits` section of the release notes - not too helpful
3. I've made a [component library](https://gitlab.com/benny.m/ci_components) for our CI/CD (public and my personal repo for now).
    1. This means the gitlab-ci.yml files have less repetition and can be much smaller per repo. Already this gave a reduction in the LOC from 210 -> 80 (60% reduction)
    2. Here, I've put the following steps into the component library - you can see how they're called (with inputs!) in quoting engine [here](https://gitlab.com/coverdash/quoting_engine/-/blob/release_prod/.gitlab-ci.yml?ref_type=heads) - hopefully more to come like the deploy steps
        1. Tag
        2. Release
        3. Build
4. Build (only for the component library version) now uses Nexus on `release_prod` and if your feature branch does not have a `coverdash_common` branch associated with it
    1. This speeds up build time in common by about 25% (down to 2 minutes) and helps ensure stability of releases
    2. It also means your feature branch **has** to build successfully to be approved
        1. Either it works with the nexus version of common
        2. Or it works with your branch's `coverdash_common` version
	