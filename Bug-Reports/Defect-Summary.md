# Defect Summary — Build 1.0

## Overview

During defect-focused functional testing using the `problem_user` account, all six products were individually checked by comparing the product information displayed on the Products page with the information displayed after selecting the product.

Six reproducible product-detail defects were identified.

## Defect Summary

| Defect ID | Selected Product | Incorrect Detail Displayed | Severity | Priority | Status |
|---|---|---|---|---|---|
| BUG-001 | Sauce Labs Fleece Jacket | ITEM NOT FOUND with incorrect image description and price | Major | High | Open |
| BUG-002 | Sauce Labs Backpack | Sauce Labs Fleece Jacket details | Major | High | Open |
| BUG-003 | Sauce Labs Bolt T-Shirt | Sauce Labs Onesie details | Major | High | Open |
| BUG-004 | Sauce Labs Onesie | Test.allTheThings() T-Shirt (Red) details | Major | High | Open |
| BUG-005 | Sauce Labs Bike Light | Sauce Labs Bolt T-Shirt details | Major | High | Open |
| BUG-006 | Test.allTheThings() T-Shirt (Red) | Sauce Labs Backpack details | Major | High | Open |

## Testing Account

`problem_user`

## Build

Build 1.0

## Testing Area

Product Details / Product Selection

## Overall Finding

All six products displayed incorrect product-detail information when selected using the `problem_user` account.

The defects affect product name image description and/or price and may result in customers viewing information that does not correspond to the product they selected.

## Defect Status

All six defects remain **Open** and require investigation and resolution.

## Test Case Traceability

Primary test case:

**TC-056 — Verify selected product details match the product displayed**

Associated defects:

- BUG-001
- BUG-002
- BUG-003
- BUG-004
- BUG-005
- BUG-006

## Conclusion

The product-detail functionality should not be considered fully acceptable for the affected user scenario until the identified defects are resolved and successfully retested.
