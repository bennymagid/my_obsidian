

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

To get approx and exact info on company revenue
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
    monthORDER BY  
    month ASC;  
  
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
    monthORDER BY  
    month;
```