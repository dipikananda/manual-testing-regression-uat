# BUG-005 — Sauce Labs Bike Light Displays Incorrect Product Details

## Bug Summary

The Sauce Labs Bike Light displays incorrect product details when opened using the `problem_user` account.

## Environment

| Field | Details |
|---|---|
| Application | SauceDemo |
| User | problem_user |
| Build | Build 1.0 |
| Browser | Chrome |
| Testing Type | Defect-focused Functional Testing |
| Priority | High |
| Severity | Major |
| Status | Open |

## Steps to Reproduce

1. Log in using `problem_user`.
2. Open the Products page.
3. Locate **Sauce Labs Bike Light**.
4. Note the product details.
5. Click **Sauce Labs Bike Light**.
6. Observe the product details page.

## Expected Result

The product details page should display:

- Product name: **Sauce Labs Bike Light**
- Correct Bike Light image
- Correct Bike Light description
- Price: **$9.99**

## Actual Result

The product details page displays:

- Product name: **Sauce Labs Bolt T-Shirt**
- Product image: **Blue T-Shirt image**
- Product description: **Bolt T-Shirt description**
- Price: **$15.99**

The displayed product details do not correspond to the selected Sauce Labs Bike Light.

## Impact

Customers may receive incorrect product information when selecting the Bike Light, potentially resulting in incorrect product selection.

## Reproducibility

**Reproducible:** Yes

## Defect Status

**Open — requires investigation and fix.**
## Retest Result

**Retest Result:** Failed

**Actual Result:** The same incorrect product-detail mapping remains reproducible.

**Defect Status:** Open

**Conclusion:** The defect remains unresolved and requires a fix before closure.
