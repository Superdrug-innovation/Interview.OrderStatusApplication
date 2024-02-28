# Interview Scenario
Background:
When a customer places an order on our ecommerce website, the ecom system decides which 1 of our 3 separate fulfilment system should fulfil the order. A order status application was created to query the 3 different fulfilment systems and return information on a given order. Currently the application has endpoints that can be used to query each individual system but no way to query all systems in one call.
 
Objectives:
We want you to create a new endpoint on the order status application that will query all 3 systems and then run calculations on this data and return the results.
 
Design:
The application is a dotnet 6 web API. It is a stateless system that requires no database. The system has been built following the clean code architecture and principles. It also uses the mediator library to communicate between the API layer and it's logic layer. Our team follows the BDD approach for testing.
 
Deliverables:
Create a new endpoint that query's all 3 systems, performs calculations on the data and returns the results.
Write unit tests to confirm logic and functionality of this feature.
Follow design principles and architecture used in project.
 
Timings:
We would like you to spend no more than 2 hours working on this feature.
 
 
User Stories:
As a order status application user
I want to give the application a order number and receive current status, the fulfilment time and the average pick time for the order
So that i can see where the order is, if it's late and how long it's taking to pick.
 
Acceptance criteria:
AC1
Given a order number
When I get a result from 1 of the 3 fulfilment systems
Then i return the status
 
AC2
Given a order number
When i get a result from a order number
Then i calculate the total time it took to fulfil the order
 
AC3
Given a order number
When i get a result from a order number
Then i calculate the average pick time for the order
