- Improvements to CI/CD
	- No longer need to manually (and dangerously) [allow AWS connections](https://linear.app/coverdash/issue/WEB-997/fix-having-to-add-a-new-temp-security-rule-to-aws-every-time-i-want-to) to our gitlab instance on every release - automated whitelist -- [[🚀 Changes to Release]]
- Introduced better practices with [[🏴󠁧󠁢󠁳󠁣󠁴󠁿 Lombok]] to save boilerplate
- Introduced PreHandle usage for more reusable and safer user validation
- Introduced a unified AWS Uploader that will hopefully reduce repeated (and unchecked) code interfacing with S3
- Kudos 1 month in from Perry for writing clear tickets for FE
- Led [major project](https://linear.app/coverdash/issue/WEB-2580/add-csv-importer-for-accounting) early on which involved design and has enabled faster Accountant turnaround and EOM
- Testing finally [[🍬 Testing Suite]]

- Plans
	- Clearly documented tickets and plans 
		- [AWS migration](https://linear.app/coverdash/issue/WEB-2588/upgrade-aws-s3-sdk-from-v1-v2) 
		- [User validation](https://linear.app/coverdash/issue/WEB-2595/deprecate-validationhelper) -- [[🔑 User Auth]]
		- [enums for PolicyDirection](https://linear.app/coverdash/issue/WEB-2590/replace-hardcoded-string-in-policytransaction-and)
		- Other ideas captured in [[💡Ideas for CI - CD]]
	- Dependencies(!!)
	