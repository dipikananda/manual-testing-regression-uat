# BUG-001 — Incorrect Product Details Displayed for Sauce Labs Fleece Jacket

## Bug Summary

The Sauce Labs Fleece Jacket product displays incorrect product information when opened using the `problem_user` account.

## Environment

| Field | Details |
|---|---|
| Application | SauceDemo |
| URL | https://www.saucedemo.com/ |
| User | problem_user |
| Password | secret_sauce |
| Build | Build 1.0 |
| Browser | Chrome |
| Testing Type | Defect-focused Functional Testing |
| Priority | High |
| Severity | Major |
  Status | Open - Failed Test Case TC-056

## Preconditions

- SauceDemo application is accessible.
- User is logged in using `problem_user`.
- Products page is displayed.

## Steps to Reproduce

1. Log in using `problem_user`.
2. Open the Products page.
3. Locate **Sauce Labs Fleece Jacket**.
4. Click **Sauce Labs Fleece Jacket**.
5. Observe the product details page.

## Expected Result

After selecting **Sauce Labs Fleece Jacket**, the product details page should display:

- Product name: **Sauce Labs Fleece Jacket**
- Correct product image
- Correct product description
- Correct product price

## Actual Result

After selecting **Sauce Labs Fleece Jacket**, the product details page displays:

- Product name: **ITEM NOT FOUND**
- Product image: **Dog image**
- Product description does not match **Sauce Labs Fleece Jacket**
- Product price does not match **Sauce Labs Fleece Jacket**

The product details displayed do not correspond to the product selected by the user.

## Evidence

The defect was reproduced manually during Build 1.0 testing using the `problem_user` account.

## Impact

Customers using the affected account may see incorrect product information after selecting a product. This can reduce confidence in the product catalog and may result in incorrect product selection.

## Reproducibility

**Reproducible:** Yes

## Defect Status

**Open — requires investigation and fix.**
## Linked Test Case

**TC-056 — Verify selected product details match the product displayed**

**Execution Result:** Failed

**Defect ID:** BUG-001

## Defect Lifecycle

**Open → Fix Required → Retest Pending**
