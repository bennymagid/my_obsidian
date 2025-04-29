1) Coverdash is an insurance broker that allows small businesses to receive insurance quotes through a streamlined online experience. To get quotes, we must submit an application containing the user’s business information to a dozen or more insurance carriers, each via their own REST API.
 
Each carrier has its own API with unique request / response formats. Each carrier interaction may take different amounts of time or may fail altogether. 

(Assuming that we have already collected all of the user's business information). Design the Quoting Engine, the backend service that is responsible for:
1. Submitting the application to all configured carrier APIs in parallel
2. Waiting for all responses (or timeouts/failures)
3. (Saving the carrier responses)

Be sure to also discuss how the frontend fits into your design.

2) Discuss how Coverdash should store Businesses in our database. Keep in mind that businesses may have multiple Applications, Users, Addresses, etc.

