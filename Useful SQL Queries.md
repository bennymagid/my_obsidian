

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
    p."createdAt" >= '2024-01-01' AND p."createdAt" < '2025-01-01'  
    AND a.type = 'location'  
  
GROUP BY  
    a.state  
ORDER BY  
    total_premium DESC;
```