In `Cursor` navigate to the correct front-end branch in the `admin-dashboard` project.

Must specify which service is local vs remote at the top of the `.env.local-backend` file. Here, we use LAQ, but you'll generally use `localhost:8083` for crud

```
# -- UAT ENV --

NEXT_PUBLIC_QUOTING_ENGINE_URL=https://lb-quoting-engine-uat.coverdash.com

NEXT_PUBLIC_SERVICE_MANAGER_URL=https://lb-service-manager-uat.coverdash.com

NEXT_PUBLIC_CRUD_SERVICE_URL=https://lb-crud-uat.coverdash.com

NEXT_PUBLIC_PARTNER_DASHBOARD_SERVICE_URL=https://lb-partner-dashboard-service-uat.coverdash.com

NEXT_PUBLIC_PARTNER_SERVICE_URL=https://lb-partner-service-uat.coverdash.com

NEXT_PUBLIC_LAQ_SERVICE_URL=https://localhost:8088 #https://lb-lead-assignment-service-uat.coverdash.com
```

Then run the local backend to test and then  `yarn local-backend` 