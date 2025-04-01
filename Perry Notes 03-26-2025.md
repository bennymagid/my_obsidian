1. Above, in the summary of our meeting, it says: When the user purchases, a webhook will be triggered that sends you all the policy information (the link to our dashboard, a link to the COI, pricing, etc.)
However, in the documentation, we could not find anything about this. Please send us the URL of where we can find the information about the webhook.
We have information about the getPoliciesByBusiness API but that doesn't inform us of a new purchase.
2. Above, it says: When the user purchases, we will give you the HTML that will listen to the iframe to notify your UI as well.
We need more information about what this HTML is - we need to review it from a security perspective, to make sure it can be included on our page.
Answer for 1 and 2:
It's technically a "callback" that the browser HTML/JS needs to listen for. As part of the HTML code example we will provide, this listener will be included as Javascript code. This callback provides the policy ID. To get more info such as a link to the COI, our API will need to be called using the business ID that you already have saved. See the `getPoliciesByBusinessId` endpoint in our docs.
3. If we use the webhook, will we get it for each policy that is purchased by the customer?
Yes, when the listener + getPoliciesByBusinessId API is set up together, this data will be sent every time a customer purchases a policy.
4. Will be get a webhook upon renewal? How do we identify a policy as a purchase or renewal?
Not sure if we generally tell partners anything about renewals besides for them being able to view it in their metrics.
5. Can you give us the contact info of where our customer service should send customers that need Coverdash suppose?
Customers will have a Coverdash Account portal they can access.  This provides them with policy info, COI functionality, claims management, and support resources including live chat.
6. If a customer cancels a policy with Coverdash, are we informed of the cancellation? How?
Cancellations are handled entirely by our Operations team.
7. What if a customer cancels his iPostal1 account - how will he be able to get access to his Coverdash policies, once he no longer has access to our portal?
Yes, all current and previous Coverdash customers will always have access to their Coverdash Account online portal.
8. Re opening a coverdash account - the documentation says we will send an email and business name. We prefer to send a unique identifier instead. Is that acceptable?
Since we have no mapping of iPostal's unique identifiers to actual business names and customer info, unfortunately, this is not something we can do at this time.