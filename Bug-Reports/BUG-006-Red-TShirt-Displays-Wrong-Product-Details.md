# BUG-006 — Test.allTheThings() T-Shirt Displays Incorrect Product Details

## Bug Summary

The Test.allTheThings() T-Shirt (Red) displays incorrect product details when opened using the `problem_user` account.

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
3. Locate **Test.allTheThings() T-Shirt (Red)**.
4. Note the product details.
5. Click **Test.allTheThings() T-Shirt (Red)**.
6. Observe the product details page.

## Expected Result

The product details page should display:

- Product name: **Test.allTheThings() T-Shirt (Red)**
- Correct T-Shirt image
- Correct T-Shirt description
- Price: **$15.99**

## Actual Result

The product details page displays:

- Product name: **Sauce Labs Backpack**
- Product image: **Backpack image**
- Product description: **Backpack description**
- Price: **$29.99**

The displayed product details do not correspond to the selected product.

## Impact

Customers may receive incorrect product information when selecting the Test.allTheThings() T-Shirt, potentially resulting in incorrect product selection.

## Reproducibility

**Reproducible:** Yes

## Defect Status

**Open — requires investigation and fix.**
