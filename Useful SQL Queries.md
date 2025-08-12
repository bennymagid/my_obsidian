To ensure correct distribution of campaigns per employee / account executive team type:
```
SELECT e.name, e."employeeType", e.team, cs."partnerId",  COUNT(c."campaignStatusId") from "EmployeeContactInformation" e  
    JOIN "CampaignEmployeeDetails" c ON e.id = c."employeeContactInformationId"  
                                                                      JOIN "CampaignStatus" cs on c."campaignStatusId" = cs.id  
WHERE e."employeeType" = 'Account Executive'  
GROUP BY e.name, e."employeeType", e.team, cs."partnerId"
```

Proportion of Bound premium per carrier per month
```
WITH monthly_totals AS (  
  SELECT  
    DATE_TRUNC('month', "createdAt") AS month,  
    SUM(premium) AS total_premium  
  FROM "Policy"  
  WHERE status = 'BOUND'  
  GROUP BY month  
),  
carrier_monthly AS (  
  SELECT  
    "carrierId",  
    DATE_TRUNC('month', "createdAt") AS month,  
    SUM(premium) AS carrier_premium  
  FROM "Policy"  
  WHERE status = 'BOUND'  
  GROUP BY month, "carrierId"  
)  
SELECT  
  cm."carrierId",  
  cm.month,  
  cm.carrier_premium,  
  mt.total_premium,  
  CAST((cm.carrier_premium / mt.total_premium * 100) * 100 AS INTEGER) / 100.0 AS percentage_of_month,  
  CAST((cm.carrier_premium / mt.total_premium) * 10000 AS INTEGER) / 10000.0 AS proportion_of_month  
FROM carrier_monthly cm  
JOIN monthly_totals mt ON cm.month = mt.month  
ORDER BY cm.month, cm."carrierId";
```

CYBER conversion rate 
```
SELECT DISTINCT pt.id                AS transaction_id,  
                pt.amount            AS amount,  
                pt.direction         AS direction,  
                pt."createdAt"       AS transaction_created_at,  
                pt."transactionType" AS transaction_type,  
                pt."totalAmount"     AS total_amount,  
                p.id                 AS policy_id,  
                p."externalPolicyId" AS external_policy_id,  
                p.premium            AS premium,  
                p."carrierId"        AS carrier_id,  
                p."policyType"       AS policy_type,  
                p."createdAt"        AS policy_created_at,  
                p."effectiveDate"    AS effective_date,  
                p."expiryDate"       AS expiryDate,  
                p."cancellationDate" AS cancellation_date,  
                p.status             AS status,  
                p."commissionRate"   AS commisssion_rate,  
                a.state              AS state,  
                p."licenseName"      AS license_name,  
                p."policyType"       AS policy_type,  
                p."saleType"         AS sale_type  
FROM "PolicyTransaction" pt  
         LEFT JOIN "Policy" p ON pt."policyId" = p.id  
         LEFT JOIN (SELECT DISTINCT ON ("businessId") *  
                    FROM "BusinessLocation"  
                    ORDER BY "businessId", "createdAt" DESC) bl ON p."businessId" = bl."businessId"  
         LEFT JOIN "Address" a ON bl.id = a."businessLocationId" AND a.type = 'location'  
WHERE p."createdAt" >= DATE '2023-01-01'  
  AND p."createdAt" < DATE '2025-06-01';
```

Policy Transaction info dump
```
SELECT DISTINCT pt.id                AS transaction_id,  
                pt.amount            AS amount,  
                pt.direction         AS direction,  
                pt."createdAt"       AS transaction_created_at,  
                pt."transactionType" AS transaction_type,  
                pt."totalAmount"     AS total_amount,  
                p.id                 AS policy_id,  
                p."externalPolicyId" AS external_policy_id,  
                p.premium            AS premium,  
                p."carrierId"        AS carrier_id,  
                p."policyType"       AS policy_type,  
                p."createdAt"        AS policy_created_at,  
                p."effectiveDate"    AS effective_date,  
                p."expiryDate"       AS expiryDate,  
                p."cancellationDate" AS cancellation_date,  
                p.status             AS status,  
                p."commissionRate"   AS commisssion_rate,  
                a.state              AS state,  
                p."licenseName"      AS license_name,  
                p."saleType"         AS sale_type  
FROM "PolicyTransaction" pt  
         LEFT JOIN "Policy" p ON pt."policyId" = p.id  
         LEFT JOIN (SELECT DISTINCT ON ("businessId") *  
                    FROM "BusinessLocation"  
                    ORDER BY "businessId", "createdAt" DESC) bl ON p."businessId" = bl."businessId"  
         LEFT JOIN "Address" a ON bl.id = a."businessLocationId" AND a.type = 'location'  
WHERE p."createdAt" >= DATE '2023-01-01'  
  AND p."createdAt" < DATE '2025-07-01';
```

To add a new employee to growth campaigns
```
WITH cnts AS (SELECT "CampaignEmployeeDetails"."campaignStatusId", COUNT(*) AS cnt FROM "CampaignEmployeeDetails" GROUP BY "campaignStatusId")  
  
INSERT INTO "CampaignEmployeeDetails" (id, "employeeContactInformationId", "campaignStatusId")  
SELECT  
  gen_random_uuid(),  
  60,  
  campaignId  
FROM (SELECT "campaignStatusId" FROM cnts WHERE cnt > 2) AS campaignIds(campaignId)
```

To add a new campaign for all employees in growth (add to list of employees as necessary)
```
INSERT INTO "CampaignEmployeeDetails" (id, employeeContactInformationId, campaignStatusId)
SELECT
  gen_random_uuid(),
  employee_id,
  'your-new-campaign-status-id-here'
FROM (
  VALUES
    (51),
    (54),
    (15),
    (55),
    (9),
    (39),
    (34),
    (23),
    (49),
    (46),
    (20),
    (41)
) AS employee_ids(employee_id);
```

Get the total revenue per state for 2024 (imperfect because `Address.state` isn't perfect)

```
SELECT  
    a.state,  
    SUM(p.premium) AS total_premium,  
    COUNT(DISTINCT p.id) AS accounts_sold  
FROM  
    "Policy" p  
JOIN  
    "Business" b ON p."businessId" = b.id  
JOIN  
    "BusinessLocation" bl ON b.id = bl."businessId"  
JOIN  
    "Address" a ON a."businessLocationId" = bl."id"  
WHERE  
    p."createdAt" >= '2024-01-01' 
    AND p."createdAt" < '2025-01-01'  
    AND a.type = 'location'  
  
GROUP BY  
    a.state  
ORDER BY  
    total_premium DESC;
```


To get the total revenue for a given agent for a certain time

```
SELECT  
  b."soldBy",  
  SUM(  
    CASE  
      WHEN pt."direction" = 'RECEIVABLE' THEN pt."amount"  
      WHEN pt."direction" = 'PAYABLE' THEN -pt."amount"  
      ELSE 0  
    END  
  ) AS amount  
FROM  
  "Business" b  
JOIN  
  "Policy" p ON b.id = p."businessId"  
JOIN  
  "PolicyTransaction" pt ON p.id = pt."policyId"  
WHERE  
  b."soldBy" IN ('William Haskell', 'Jake Kehl')  
  AND p."saleType" = 'NEW_BUSINESS'  
  AND p."createdAt" >= '2025-04-01'  
  AND p."createdAt" < '2025-05-01'  
  AND pt."transactionType" IN ('TECHNOLOGY_ACCESS_FEE', 'COMMISSION')  
GROUP BY  
  b."soldBy";
```

To get approx (only premium-based) OR exact info on company revenue
```
SELECT  
    DATE_TRUNC('month', p."createdAt") AS month,  
    SUM(p.premium * p."commissionRate") AS rev,  
    COUNT(DISTINCT p.id) AS accounts_sold  
FROM  
    "Policy" p  
WHERE  
    p."createdAt" >= NOW() - INTERVAL '12 months'  
GROUP BY  
    month
ORDER BY  
    month ASC;  

//----
  
SELECT  
    DATE_TRUNC('month', pt."createdAt") AS month,  
    SUM(  
    CASE  
      WHEN pt."direction" = 'RECEIVABLE' THEN pt."amount"  
      WHEN pt."direction" = 'PAYABLE' THEN -pt."amount"  
      ELSE 0  
    END  
  ) AS amount  
FROM  
    "PolicyTransaction" pt  
WHERE  
    pt."createdAt" >= NOW() - INTERVAL '12 months'  
GROUP BY  
    month
ORDER BY  
    month;
```