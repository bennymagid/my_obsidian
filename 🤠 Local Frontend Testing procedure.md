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

Could figure out a way to automate this in our [[🍬 Testing Suite]]?


**make sure to change the prod properties file if running PROD** (in crud)
(this is copied from local properties)

```
%% CHANGE  %spring.datasource.hikari.maximum-pool-size=3%
server.port=8083
security.require-ssl=true
server.ssl.key-store-type=PKCS12
server.ssl.key-store=certificate_local.p12
server.ssl.key-store-password=Coverdash233%%$$##@@
```


To run frontend locally
- Open `admin-dashboard` frontend
- run backend crud-service - there's a local cert that makes this work
- run `yarn local-backend` (uses `.env.local.backend.`)