# Swag Labs — Cart Test Cases

## TC-CART-001 — Add a product to the cart

| Field | Details |
|---|---|
| Test Case ID | TC-CART-001 |
| Title | Verify that a user can add a product to the shopping cart |
| Priority | High |
| Preconditions | The user is logged in to Swag Labs |
| Test Data | Product: `Sauce Labs Backpack` |
| Steps | 1. Click **Add to cart** for `Sauce Labs Backpack`.<br>2. Verify that the cart badge displays `1`.<br>3. Click the cart icon. |
| Expected Result | The cart badge displays `1` and `Sauce Labs Backpack` is displayed in the cart. |
| Actual Result | The cart badge displayed `1` and `Sauce Labs Backpack` was displayed in the cart. |
| Status | Passed |

---

## TC-CART-002 — Remove a product from the cart

| Field | Details |
|---|---|
| Test Case ID | TC-CART-002 |
| Title | Verify that a user can remove a product from the shopping cart |
| Priority | High |
| Preconditions | The user is logged in and `Sauce Labs Backpack` is in the cart |
| Steps | 1. Open the cart.<br>2. Click **Remove** for `Sauce Labs Backpack`. |
| Expected Result | The product is removed from the cart and the cart badge is no longer displayed. |
| Actual Result | The product was removed from the cart and the cart badge was no longer displayed. |
| Status | Passed |
