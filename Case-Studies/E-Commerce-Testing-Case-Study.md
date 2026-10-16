
# E-commerce Website Testing Case Study

## 1. Project Overview

- **Project:** E-commerce Website — Portfolio Demonstration
- **Role:** QA Engineer
- **Testing Type:** Functional, Integration, Regression, and UI Testing
- **Status:** Test design completed; execution not performed
- **Application:** Hypothetical demo application

## 2. Business Scenario

An online shopping application allows customers to browse
products, search for items, add products to a cart, apply
discount codes, complete checkout, and view order details.

The objective is to identify risks that could prevent
customers from placing correct orders or receiving accurate
pricing and order information.

## 3. Scope of Testing

### In Scope
- Product listing and search
- Product details and availability
- Add to cart and remove from cart
- Quantity updates
- Price, tax, shipping, and discount calculations
- Checkout form validation
- Order confirmation
- Order history
- Session behavior during shopping

### Out of Scope
- Production payment transactions
- Live customer data
- Performance testing
- Third-party systems not available in the test environment

## 4. Risk-Based Test Priorities

| Feature | Risk | Priority | Reason |
|---|---|---|---|
| Checkout | High | P1 | Customers may be unable to place orders |
| Price calculation | High | P1 | Incorrect totals can cause financial impact |
| Cart updates | High | P1 | Incorrect quantities affect orders |
| Payment result handling | High | P1 | Incorrect order/payment status is serious |
| Product search | Medium | P2 | Customers may struggle to find products |
| Product images | Low | P3 | Visual issues may affect usability |

## 5. Sample Test Scenarios

| Test Case ID | Scenario | Expected Result | Priority |
|---|---|---|---|
| ECOM_001 | Search for an existing product | Relevant products are displayed | P1 |
| ECOM_002 | Search for a nonexistent product | A useful no-results message appears | P2 |
| ECOM_003 | Open a product details page | Correct product details are displayed | P1 |
| ECOM_004 | Add an available product to cart | Product is added with correct quantity | P1 |
| ECOM_005 | Increase cart quantity | Quantity and subtotal update correctly | P1 |
| ECOM_006 | Remove a cart item | Item is removed and totals recalculate | P1 |
| ECOM_007 | Enter an invalid discount code | Code is rejected with appropriate feedback | P2 |
| ECOM_008 | Enter an expired discount code | Discount is not applied | P2 |
| ECOM_009 | Submit checkout with missing required fields | Validation is displayed | P1 |
| ECOM_010 | Submit valid shipping details | Checkout proceeds to the next valid step | P1 |
| ECOM_011 | Verify order total | Subtotal, discount, tax, and shipping follow the pricing rules | P1 |
| ECOM_012 | Refresh the cart page | Cart behavior follows the defined persistence rules | P2 |
| ECOM_013 | Attempt to order an unavailable product | Order is prevented or availability is handled correctly | P1 |
| ECOM_014 | Complete an order using an approved payment sandbox | Order and payment statuses are consistent | P1 |
| ECOM_015 | Refresh the order confirmation page | Duplicate orders are not created | P1 |

## 6. Test Data

Use fictional data only.

- Product: Demo Wireless Mouse
- Product price: 500 currency units
- Quantity: 2
- Sample discount: 10%, if supported by the demo
- Customer: qa.demo@example.com
- Shipping address: Authorized synthetic test address

Actual totals must be calculated according to the application's
documented tax, shipping, and discount rules.

## 7. Defect Reporting Approach

For each confirmed issue, record:

- Unique defect ID
- Clear title and description
- Preconditions and reproducible steps
- Expected and actual results
- Severity and priority
- Environment and supporting evidence
- Status and retest result

## 8. Exit Criteria

- Planned test cases have been executed or exceptions documented.
- Critical order and pricing defects are resolved or formally accepted.
- Test results and outstanding risks are communicated.
- Order and payment status consistency is verified.

## 9. Current Status

This is a hypothetical portfolio case study.

No live application has been tested. All scenarios are
proposed test designs, not verified results.

## 10. Conclusion

This case study demonstrates risk-based thinking across
product discovery, cart management, checkout, pricing,
and order processing.

The next step would be execution against an authorized
demo application, followed by actual results and defect reports.
