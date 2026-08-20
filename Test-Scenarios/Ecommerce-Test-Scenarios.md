# Test Scenarios – SauceDemo Release, Regression and UAT Testing

## 1. Smoke Testing Scenarios

Smoke testing will verify that the critical application functions are available and stable before detailed testing begins.

| Scenario ID | Scenario | Expected Outcome |
|---|---|---|
| TS-SM-001 | Verify the application loads successfully | Login page should be displayed |
| TS-SM-002 | Verify user can log in with valid credentials | Products page should be displayed |
| TS-SM-003 | Verify products are displayed after login | Product list should be displayed correctly |
| TS-SM-004 | Verify a product can be added to the shopping cart | Selected product should appear in the cart |
| TS-SM-005 | Verify checkout workflow can be initiated | Checkout information page should be displayed |

### Smoke Testing Objective

The smoke test suite provides a quick assessment of the application's critical functionality. If a critical smoke test fails, detailed testing may be paused until the build is considered stable.
## 2. Functional Testing Scenarios

Functional testing will verify that the application's features behave according to the expected functional requirements.

| Scenario ID | Scenario | Expected Outcome |
|---|---|---|
| TS-FN-001 | Verify valid user login | User should successfully log in |
| TS-FN-002 | Verify invalid username/password handling | Appropriate error message should be displayed |
| TS-FN-003 | Verify product names are displayed correctly | Product names should be visible and correct |
| TS-FN-004 | Verify product prices are displayed correctly | Product prices should be displayed correctly |
| TS-FN-005 | Verify product descriptions are displayed | Product descriptions should be available |
| TS-FN-006 | Verify product sorting by name A to Z | Products should be sorted alphabetically |
| TS-FN-007 | Verify product sorting by name Z to A | Products should be sorted in reverse alphabetical order |
| TS-FN-008 | Verify product sorting by price low to high | Products should be sorted from lowest to highest price |
| TS-FN-009 | Verify product sorting by price high to low | Products should be sorted from highest to lowest price |
| TS-FN-010 | Verify a product can be added to the cart | Selected product should appear in the cart |
| TS-FN-011 | Verify multiple products can be added to the cart | All selected products should appear in the cart |
| TS-FN-012 | Verify a product can be removed from the cart | Selected product should be removed |
| TS-FN-013 | Verify cart quantity is displayed correctly | Cart should show the correct quantity |
| TS-FN-014 | Verify valid checkout information can be submitted | User should proceed to order overview |
| TS-FN-015 | Verify an order can be successfully placed | Order confirmation should be displayed |

### Functional Testing Objective

The functional test scenarios provide detailed coverage of the application's core business functions and will also provide the baseline for later regression testing.
## 3. Negative Testing Scenarios

Negative testing will verify how the application handles invalid, incomplete or unexpected user input.

| Scenario ID | Scenario | Expected Outcome |
|---|---|---|
| TS-NT-001 | Verify login with blank username and password | Appropriate validation/error message should be displayed |
| TS-NT-002 | Verify login with invalid username | Appropriate error message should be displayed |
| TS-NT-003 | Verify login with invalid password | Appropriate error message should be displayed |
| TS-NT-004 | Verify checkout with blank first name | First Name validation message should be displayed |
| TS-NT-005 | Verify checkout with blank last name | Last Name validation message should be displayed |
| TS-NT-006 | Verify checkout with blank postal code | Postal Code validation message should be displayed |
| TS-NT-007 | Verify checkout with all mandatory fields blank | Appropriate validation message should be displayed and user should not proceed |
| TS-NT-008 | Verify removing a product from an empty cart | Application should handle the action appropriately without breaking the workflow |

### Negative Testing Objective

The negative test scenarios will verify that invalid or incomplete user actions are handled correctly and that appropriate validation or error messages are displayed.
## 4. Retesting Scenarios

Retesting will be performed after defects identified during the initial test cycle have been addressed. The original failed test cases will be executed again to verify that the reported defects have been resolved.

| Scenario ID | Scenario | Expected Outcome |
|---|---|---|
| TS-RT-001 | Retest previously failed login functionality after defect fix | Previously failed login test should now pass |
| TS-RT-002 | Retest previously failed product functionality after defect fix | Previously failed product test should now pass |
| TS-RT-003 | Retest previously failed cart functionality after defect fix | Previously failed cart test should now pass |
| TS-RT-004 | Retest previously failed checkout functionality after defect fix | Previously failed checkout test should now pass |
| TS-RT-005 | Retest previously failed order placement functionality after defect fix | Previously failed order placement test should now pass |

### Retesting Objective

The objective of retesting is to confirm that previously identified defects have been successfully resolved.

Retesting will focus only on the specific failed functionality associated with the reported defect.

A retest will be marked as:

- **Pass** – The original defect is no longer reproducible and the expected result is achieved.
- **Fail** – The defect remains reproducible or the expected result is still not achieved.

Retesting results will be linked to the relevant Test Case ID and Bug ID in the Test Execution documentation.
