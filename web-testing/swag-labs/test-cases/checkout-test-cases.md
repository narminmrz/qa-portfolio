# Swag Labs — Checkout Test Cases

## TC-CHECKOUT-001 — Checkout attempt with an empty First Name

| Field | Details |
|---|---|
| Test Case ID | TC-CHECKOUT-001 |
| Title | Verify that checkout cannot continue when First Name is empty |
| Priority | High |
| Preconditions | The user is logged in, a product is in the cart, and the Checkout: Your Information page is open |
| Test Data | First Name: empty / Last Name: empty / Postal Code: empty |
| Steps | 1. Click **Checkout** from the cart.<br>2. Leave all fields empty.<br>3. Click **Continue**. |
| Expected Result | The user remains on the information page and a First Name required error message is displayed. |
| Actual Result | The user remained on the information page and the following message was displayed: `Error: First Name is required` |
| Status | Passed |


---

## TC-CHECKOUT-002 — Complete checkout with valid information

| Field | Details |
|---|---|
| Test Case ID | TC-CHECKOUT-002 |
| Title | Verify that a user can complete checkout with valid information |
| Priority | High |
| Preconditions | The user is logged in, a product is in the cart, and the Checkout: Your Information page is open |
| Test Data | First Name: `Test` / Last Name: `User` / Postal Code: `AZ1000` |
| Steps | 1. Enter valid first name, last name, and postal code.<br>2. Click **Continue**.<br>3. Verify the product and price on the overview page.<br>4. Click **Finish**. |
| Expected Result | The checkout is completed successfully and an order confirmation message is displayed. |
| Actual Result | The checkout was completed successfully and the following message was displayed: `Thank you for your order!` |
| Status | Passed |
