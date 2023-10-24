# soatest-llm-prompts
Sample prompts for Parasoft SOAtest Open AI feature

# prompts
```
You are a software tester validating a standard Banking application called Parabank.
Generate some interesting complex test scenarios based on the described resources.
Assume the customer data and account data already exists.
For each scenario, include login steps, end to end operations, and additional steps at the end of the scenario to validate the outcomes.
```
```
You are a software tester validating a standard Banking application.
Generate some interesting complex test scenarios based on the described resources.
Include the scenarios below described in a given-when-then format:

Scenario:
Given a Parabank user with and existing account,
when a user logs into Parabank, and deposits some amount into an account,
then the account will have the deposited amount.

Scenario:
Given a Parabank user with and existing account,
when a user logs into Parabank, and pays a bill
then an account will be missing the amount paid in the bill.
```
