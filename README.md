# SOAtest LLM prompts
Sample prompts for Parasoft SOAtest Open AI feature

# Test scenario craeation prompts
Natural language example
```
You are a software tester validating a standard Banking application called Parabank.
Generate some interesting complex test scenarios based on the described resources.
Assume the customer data and account data already exists.
For each scenario, include login steps, end to end operations, and additional steps at the end of the scenario to validate the outcomes.
```
BDD example
```
You are a software tester validating a standard Banking application.
Generate some interesting complex test scenarios based on the described resources.
Include the scenarios below described in a given-when-then format:

Scenario:
Given a Parabank user with an existing account,
when a user logs into Parabank, and deposits some amount into an account,
then the account will have the deposited amount.

Scenario:
Given a Parabank user with an existing account,
when a user logs into Parabank, and pays a bill
then an account will be missing the amount paid in the bill.

```
# AI Assistant prompts
## Test scenarios with data source and paramterization for submit order flow
1)
```
Using the REST API <demo-app-url>/pda/api-docs/v1-proxy, please create a test scenario to validate this flow:

given two items added to the cart, 
when user submits the order
then verify that the order has been placed.

Please parameterize the set of items added to the cart. 
Please also parameterize the region. 
I would like 5 columns - two columns have item ids randomly selected between 1 and 9. 
Two columns have random quantities between 1 and 5. 
One column represents region and should be set to "LOCATION_1" for all rows. There should be 10 rows.
```
2)
```
Please create a test scenario from <demo-app-url>/pda/api-docs/v1. 
The scenario should 
add a new asset category, 
check the category was added, 
add two items to each new category.

Please create a data source for me.
Parameterize the scenario to parameterize the set of new asset categories, as well as each of the items added for each category. 
I would like columns for asset 
category name, 
asset category description, 
asset category image path where the values are defined like "/uploaded_images/outdoor/category1.jpg", 
first asset name, 
first asset description, first asset in stock (integer), 
second asset name, 
second asset description, 
second asset in stock (integer), 
and a region column that's the same for both assets. 

Please use asset categories and items that are related to backpacking, excluding tents, backpacks, and sleeping bags. 
Each category description should be 2 sentences, and each asset description should be 1 sentence. Region should use "LOCATION_1" for every row. Please create 4 rows of data.



