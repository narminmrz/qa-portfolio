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
