# BUG-002 — Sauce Labs Backpack Displays Incorrect Product Details

## Bug Summary

The Sauce Labs Backpack displays incorrect product details when opened using the `problem_user` account.

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

## Preconditions

- SauceDemo application is accessible.
- User is logged in using `problem_user`.
- Products page is displayed.

## Steps to Reproduce

1. Log in using `problem_user`.
2. Open the Products page.
3. Locate **Sauce Labs Backpack**.
4. Note the product name price description and image.
5. Click **Sauce Labs Backpack**.
6. Observe the product details page.

## Expected Result

The product details page should display the correct information for Sauce Labs Backpack:

- Product name: **Sauce Labs Backpack**
- Correct Backpack image
- Correct Backpack description
- Price: **$29.99**

## Actual Result

The product details page displays incorrect information:

- Product name: **Sauce Labs Fleece Jacket**
- Product image: **Dog image**
- Product description: **Sauce Labs Fleece Jacket description**
- Price: **$49.99**

The displayed product details do not correspond to the selected Sauce Labs Backpack.

## Impact

Customers may receive incorrect product information when selecting the Sauce Labs Backpack. This could lead to incorrect product selection and loss of confidence in the product catalogue.

## Reproducibility

**Reproducible:** Yes

## Defect Status

**Open — requires investigation and fix.**
