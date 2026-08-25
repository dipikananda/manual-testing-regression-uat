# BUG-003 — Sauce Labs Bolt T-Shirt Displays Incorrect Product Details

## Bug Summary

The Sauce Labs Bolt T-Shirt displays incorrect product details when opened using the `problem_user` account.

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
3. Locate **Sauce Labs Bolt T-Shirt**.
4. Note the product details.
5. Click **Sauce Labs Bolt T-Shirt**.
6. Observe the product details page.

## Expected Result

The product details page should display:

- Product name: **Sauce Labs Bolt T-Shirt**
- Correct Bolt T-Shirt image
- Correct Bolt T-Shirt description
- Price: **$15.99**

## Actual Result

The product details page displays:

- Product name: **Sauce Labs Onesie**
- Product image: **Sauce Labs Onesie image**
- Product description: **Sauce Labs Onesie description**
- Price: **$7.99**

The displayed product details do not correspond to the selected Sauce Labs Bolt T-Shirt.

## Impact

Customers may receive incorrect product information when selecting the Bolt T-Shirt, potentially resulting in incorrect product selection.

## Reproducibility

**Reproducible:** Yes

## Defect Status

**Open — requires investigation and fix.**
## Retest Result

**Retest Result:** Failed

**Actual Result:** The same incorrect product-detail mapping remains reproducible.

**Defect Status:** Open

**Conclusion:** The defect remains unresolved and requires a fix before closure.
