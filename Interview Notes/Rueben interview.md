Capital technology group
Speaks really well for himself
January 2026 graduation
Perfect background match

Can you select which carriers you want to interact with?

Idea: Q1 how would you handle different formats for each carrier. Assume we know what the format ought to be
A1 Java class to take in the carrier and the Business info (better, interface)

Q2 interact with the carriers. Translation layer. Different formats(!)
a. Error 
b. Timeout
c. Happy path success (with data object)

Q3 multiple carriers at the same time
try catch to wait for any carrier

Q4 thread for the FE to communicate the backend

Q5 auditing the information in our database. 
Cols: Carrier, type of response (enum), json response, json request

Q6 Quote table - what should primary key be? Carrier, customer (business)

He asked a good question about whether POST or not
