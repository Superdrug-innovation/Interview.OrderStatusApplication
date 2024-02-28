# **Interview Scenario**
## **Background:**
When a customer places an order on our e-commerce website, the e-commerce system decides which 1 of our 3 separate fulfilment systems should fulfil the order. An order status application was created to query the 3 different fulfilment systems and return information on a given order. Currently, the application has endpoints that can be used to query each system but no way to query all systems in one call.
 
## Objectives:
We want you to create a new endpoint on the order status application that will query all 3 systems and then run calculations on this data and return the results.
 
## Design:
The application is a dotnet 6 web API. It is a stateless system that requires no database. The system has been built following the clean code architecture and principles. It also uses the mediator library to communicate between the API layer and its logic layer. Our team follows the BDD approach for testing.
 
## Deliverables:
Create a new endpoint that queries all 3 systems, performs calculations on the data and returns the results.
Write unit tests to confirm the logic and functionality of this feature.
Follow design principles and architecture used in this project.
 
## Timings:
We would like you to spend no more than 2 hours working on this feature.

---

## User Stories:
As an order status application user
I want to give the application an order number and receive the current status, the fulfilment time and the average pick time for the order
So that I can see where the order is, if it's late and how long it's taking to pick.
 
### Acceptance criteria:

**AC1**\
Given an order number\
When I get a result from 1 of the 3 fulfilment systems\
Then I return the status
 
**AC2**\
Given an order number\
When I get a result from an order number\
Then I calculate the total time it took to fulfil the order
 
**AC3**\
Given an order number\
When I get a result from an order number\
Then I calculate the average pick time for the order
