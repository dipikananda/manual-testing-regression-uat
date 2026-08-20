# Test Plan – SauceDemo Release, Regression and UAT Testing

## 1. Document Overview

| Item | Details |
|---|---|
| Project | SauceDemo Release, Regression and UAT Testing |
| Application | SauceDemo E-commerce Application |
| Testing Approach | Manual Testing |
| Testing Level | System Testing |
| Primary Objective | Validate application stability across a simulated release cycle |
| Test Cycle | Build 1.0 → Build 1.1 |
| Planned Test Cases | Approximately 55 |
| Defect Management | Bug identification, reporting, retesting and closure |
| UAT | Included |

---

## 2. Test Objective

The objective of this project is to evaluate the functionality and stability of the SauceDemo e-commerce application across a simulated software release cycle.

The testing will demonstrate different QA activities, including:

- Functional Testing
- Smoke Testing
- Sanity Testing
- Retesting
- Regression Testing
- User Acceptance Testing (UAT)
- Positive Testing
- Negative Testing
- UI Testing
- Validation Testing
- Navigation Testing
- End-to-End Testing
- Defect Management

The project will simulate the lifecycle of a software change from initial build validation through defect resolution, regression testing and user acceptance.

---

## 3. Application Under Test

**Application:** SauceDemo E-commerce Application

**Application URL:** https://www.saucedemo.com/

The application provides an e-commerce workflow including:

- User login
- Product browsing
- Product details
- Product sorting
- Shopping cart
- Checkout
- Order review
- Order confirmation

---

## 4. Testing Scope

### In Scope

The following areas are included:

- Login and authentication
- Product display
- Product details
- Product sorting
- Shopping cart
- Checkout
- Order calculations
- Order placement
- Order confirmation
- Navigation
- Input validation
- Error handling
- Defect verification
- Regression of impacted functionality
- Business acceptance scenarios

### Out of Scope

The following are outside the scope of this project:

- Performance testing
- Load testing
- Stress testing
- Security penetration testing
- API testing
- Database testing
- Mobile application testing
- Automated testing

---

## 5. Testing Types and Techniques

| Testing Type / Technique | Purpose |
|---|---|
| Functional Testing | Verify application functions work according to requirements |
| Smoke Testing | Verify critical functionality is stable after a new build |
| Sanity Testing | Verify specific changes or fixes are working correctly |
| Retesting | Verify previously failed test cases pass after defect fixes |
| Regression Testing | Verify existing functionality has not been affected by changes |
| UAT | Verify the application meets defined business and user acceptance criteria |
| Positive Testing | Verify valid inputs and expected user workflows |
| Negative Testing | Verify invalid inputs and error handling |
| UI Testing | Verify user interface elements and displayed information |
| Validation Testing | Verify mandatory fields and input validation |
| Navigation Testing | Verify movement between application pages |
| End-to-End Testing | Verify the complete customer purchase workflow |
| Defect Testing | Identify, document and track application defects |

---

## 6. Test Environment

| Environment Item | Details |
|---|---|
| Application | SauceDemo |
| Environment | Web Application |
| Testing Method | Manual |
| Browser | Desktop Web Browser |
| Test Data | Valid and invalid user and checkout data |
| Build 1 | Build 1.0 – Initial Test Cycle |
| Build 2 | Build 1.1 – Post-Fix Test Cycle |

---

## 7. Test Cycle Strategy

The project will simulate two application builds.

### Build 1.0 – Initial Testing

Testing activities:

1. Smoke Testing
2. Functional Testing
3. Negative Testing
4. Defect Identification
5. Defect Reporting

Any failed test case will be documented as a defect where appropriate.

### Build 1.1 – Post-Fix Testing

After simulated defect resolution, the following activities will be performed:

1. Retesting
2. Sanity Testing
3. Regression Testing
4. UAT
5. Final Test Execution
6. Test Reporting

---

## 8. Smoke Testing Strategy

Smoke testing will focus on critical application functionality.

Examples include:

- Application loads successfully
- User can log in
- Products page is accessible
- Products can be added to the cart
- Cart can be accessed
- Checkout can be opened
- Order workflow can be initiated

If critical smoke tests fail, further testing may be stopped until the build is considered stable.

---

## 9. Retesting Strategy

Retesting will be performed on previously failed test cases after the associated defect has been addressed.

The objective is to verify:

- The original defect has been fixed
- The failed test case now passes
- The expected functionality is restored

---

## 10. Sanity Testing Strategy

Sanity testing will be performed after defect fixes to verify that the changed functionality works correctly and that the build is suitable for broader regression testing.

Sanity testing will focus on:

- The affected functionality
- Related functionality
- Critical workflows connected to the change

---

## 11. Regression Testing Strategy

Regression testing will verify that changes or defect fixes have not negatively affected existing functionality.

Regression coverage will include:

- Login
- Product browsing
- Product sorting
- Shopping cart
- Checkout
- Order calculations
- Order placement
- Order confirmation

---

## 12. UAT Strategy

User Acceptance Testing will verify that the application supports the expected business workflow from a user's perspective.

UAT will focus on the complete customer journey:

1. Login
2. Browse products
3. Select products
4. Add products to cart
5. Review cart
6. Complete checkout
7. Review order
8. Place order
9. Receive confirmation

The application will be considered acceptable when the defined acceptance criteria are satisfied.

---

## 13. Defect Management

Defects identified during testing will be documented with:

- Defect ID
- Test Case ID
- Summary
- Description
- Steps to Reproduce
- Expected Result
- Actual Result
- Severity
- Priority
- Environment
- Status

The defect lifecycle will include:

**New → Assigned → Fixed → Retest → Passed → Closed**

If a defect fails during retesting, it may be reopened.

---

## 14. Entry Criteria

Testing can begin when:

- Application is accessible
- Test environment is available
- Test data is available
- Test cases are prepared
- Build is available for testing

---

## 15. Exit Criteria

Testing can be completed when:

- Planned test cases have been executed
- Critical functionality has been tested
- Identified defects have been retested
- Regression testing has been completed
- UAT scenarios have been evaluated
- Test results have been documented
- Final test report has been prepared

---

## 16. Deliverables

The project will produce:

- Test Plan
- Test Scenarios
- Test Cases
- Smoke Test Results
- Sanity Test Results
- Retesting Results
- Regression Test Results
- UAT Results
- Test Execution Report
- Bug Reports
- Final Test Report

---

## 17. Risks and Assumptions

### Risks

- Application behavior may vary between test sessions
- Defects may not be reproducible
- Test environment availability may affect execution
- Some testing activities may depend on the application's available functionality

### Assumptions

- SauceDemo is available during testing
- Test data is available
- Testing is performed manually
- Defects are documented based on observed application behavior
- Any simulated release or defect-fix cycle will be clearly identified as simulated for portfolio purposes

---

## 18. Test Completion Criteria

The project will be considered complete when the planned testing activities have been performed and documented.

The final report will summarize:

- Total test cases
- Tests executed
- Passed tests
- Failed tests
- Defects identified
- Defects retested
- Regression results
- UAT results
- Overall release recommendation
