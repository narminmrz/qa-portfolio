# JPetStore — Cart Test Cases

## TC-CART-001 — Add an item to the cart

| Field | Details |
|---|---|
| Test Case ID | TC-CART-001 |
| Title | Verify that a user can add an item to the shopping cart |
| Priority | High |
| Preconditions | The Angelfish product detail page is open |
| Steps | 1. Click **Add to Cart** for an Angelfish item. |
| Expected Result | The item is displayed in the cart with quantity `1`. |
| Actual Result | The item was displayed in the cart with quantity `1`. |
| Status | Passed |


---

## TC-CART-002 — Update item quantity in the cart

| Field | Details |
|---|---|
| Test Case ID | TC-CART-002 |
| Title | Verify that a user can update an item quantity in the shopping cart |
| Priority | High |
| Preconditions | An item is displayed in the cart with quantity `1` |
| Steps | 1. Change the Quantity value from `1` to `2`.<br>2. Click **Update Cart**. |
| Expected Result | The item quantity is updated to `2` and the total amount is recalculated. |
| Actual Result | The item quantity was updated to `2` and the total amount increased. |
| Status | Passed |


---

## TC-CART-003 — Remove an item from the cart

| Field | Details |
|---|---|
| Test Case ID | TC-CART-003 |
| Title | Verify that a user can remove an item from the shopping cart |
| Priority | High |
| Preconditions | An item is displayed in the cart |
| Steps | 1. Click **Remove** for the item in the cart. |
| Expected Result | The item is removed and the cart is empty. |
| Actual Result | The item was removed and the cart became empty. |
| Status | Passed |
