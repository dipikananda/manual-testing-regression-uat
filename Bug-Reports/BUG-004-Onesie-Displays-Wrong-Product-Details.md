# BUG-004 — Sauce Labs Onesie Displays Incorrect Product Details

## Bug Summary

The Sauce Labs Onesie displays incorrect product details when opened using the `problem_user` account.

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
3. Locate **Sauce Labs Onesie**.
4. Note the product details.
5. Click **Sauce Labs Onesie**.
6. Observe the product details page.

## Expected Result

The product details page should display:

- Product name: **Sauce Labs Onesie**
- Correct Onesie image
- Correct Onesie description
- Price: **$7.99**

## Actual Result

The product details page displays:

- Product name: **Test.allTheThings() T-Shirt (Red)**
- Product image: **T-Shirt (Red) image**
- Product description: **T-Shirt (Red) description**
- Price: **$15.99**

The displayed product details do not correspond to the selected Sauce Labs Onesie.

## Impact

Customers may receive incorrect product information when selecting the Sauce Labs Onesie, potentially resulting in incorrect product selection.

## Reproducibility

**Reproducible:** Yes

## Defect Status

**Open — requires investigation and fix.**
