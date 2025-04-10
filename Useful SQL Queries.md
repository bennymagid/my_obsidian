

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
--   pt."transactionType",  
  SUM(pt."amount") AS total_revenue  
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
  b."soldBy"  
--        , pt."transactionType";
```