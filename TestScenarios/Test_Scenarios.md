🔹 1. Test Scenario
✅ Definition:

A Test Scenario is a high-level description of what to test.

Focuses on the feature or functionality
Does not include step-by-step details
Helps QA think of all possible paths

🔹 Key Points:
Broad / general
Covers one functionality or module
Used to identify test coverage
Easy to write early in the project

💡 Example:
Feature: Login
Test Scenarios:
-----
Valid login
Invalid login
Empty email/password
Password reset
Login with special characters
----

Feature: Add to Cart
Test Scenarios:
----
Add single product
Add multiple products
Add same product twice
Add out-of-stock product
----

✅ Definition:

A Test Case is a detailed step-by-step procedure to test a scenario. Includes inputs, actions, expected results, and actual results
Can be automated or manual

🔹 Key Points:
-Very specific
-Includes data, environment, and expected output
-Used to execute and verify functionality

💡 Example (Login Feature, scenario = Valid login):
Field	Description
Test Case ID	TC_LOGIN_01
Test Scenario	Valid Login
---
Steps	1. Open login page
2. Enter valid email
3. Enter valid password
4. Click Login button
---

Test Data	Email: test@gmail.com
Password: 123456
Expected Result	User redirected to dashboard, token received
Actual Result	(To be filled after execution)
Status	Pass / Fail

Example (Add to Cart):
Scenario: Add single product to cart
-----
Test Case:
Steps: Open homepage → Select product → Click Add to Cart
Test Data: Product ID 101
Expected Result: Product appears in cart, count = 1
----

“Test Scenarios are high-level statements of functionality to test, covering all possible conditions of a feature. 
Test Cases are detailed step-by-step instructions derived from scenarios, including inputs, expected results, and execution steps.”
----
