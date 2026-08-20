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
