Each Batch (a Businesses's batch of policies that are about to expire) can have multiple policies. Each batch is in `RenewalBatch` and each policy for a batch is in `RenewalLifeCycle`. If renewed, it will become a `RenewalPolicy`, but the old policy is a `policy`

Therefore when deleting a Business, we must recursively check through the following levels to ensure it's deleted from the RAP lifecycle:
`RenewalBatch (by businessId)` -> 
`RenewalLifeCycle (by renewalBatchId)` ->
`RenewalPolicy (by renewalLifeCycleId)`

Once the RAP lifecycle is over, the `RenewalPolicy` will be deleted and turned into a `Policy`with a type of Renewal.

![[🎤 Rap Life Cycle Overview]]