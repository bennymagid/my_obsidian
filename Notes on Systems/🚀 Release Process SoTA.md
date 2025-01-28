See Notion docs for this process up-to-date 
[here](https://www.notion.so/coverdash/Dev-Team-Best-Practices-1687c7fc5b0d80d495abfe46f8ae45d3)

We need to release to UAT, STG, and PRD all of the different relevant repos.

For a given backend repo the steps are as follows:
1. Ensure the `coverdash-common` `pom.xml` version is released and used by all other repos that reference it
2. Ensure any App Service changes are made (any column changes to be reflected)
3. Merge any changes into the release candidate branch `release/1-20-2025`
4. Pull those changes locally in IntelliJ and use Maven `package` to create a `.jar` locally
5. use Termius SFTP to copy that local `.jar`  into the corresponding remote environment. Either UAT, STG, or PRD
6. Restart the package remotely and monitor for any errors
	1. `sudo su
	2. `cd [package-name]`
	3. `./run-[package-name]`

Repos to release
1. `coverdash-common` - no need to deploy anything though
2. `crud-service
3. `coverdash_consumer
4. `lead_assignment_service
5. `partner_dashboard_service
6. `partner_service
7. `quoting_engine
8. `service_manager

With 7 repos to deploy and 3 environments, this process must be done 21 times(!)