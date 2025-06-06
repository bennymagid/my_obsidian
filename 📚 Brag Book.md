- Improvements to CI/CD
	- No longer need to manually (and dangerously) [allow AWS connections](https://linear.app/coverdash/issue/WEB-997/fix-having-to-add-a-new-temp-security-rule-to-aws-every-time-i-want-to) to our gitlab instance on every release - automated whitelist -- [[🚀 Changes to Release]]
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
	