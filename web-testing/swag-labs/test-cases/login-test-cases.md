# Swag Labs — Login Test Cases

## TC-LOGIN-001 — Successful login with valid credentials

| Field | Details |
|---|---|
| Test Case ID | TC-LOGIN-001 |
| Title | Verify that a user can log in with valid credentials |
| Priority | High |
| Preconditions | The Swag Labs login page is open |
| Test Data | Username: `standard_user` / Password: `secret_sauce` |
| Steps | 1. Enter `standard_user` in the Username field.<br>2. Enter `secret_sauce` in the Password field.<br>3. Click the **Login** button. |
| Expected Result | The user is redirected to the Products page and the product list is displayed. |
| Actual Result | The user was redirected to the Products page and the product list was displayed. |
| Status | Passed |

---

## TC-LOGIN-002 — Login attempt with an invalid username

| Field | Details |
|---|---|
| Test Case ID | TC-LOGIN-002 |
| Title | Verify that login is rejected when an invalid username is entered |
| Priority | High |
| Preconditions | The Swag Labs login page is open |
| Test Data | Username: `wrong_user` / Password: `secret_sauce` |
| Steps | 1. Enter `wrong_user` in the Username field.<br>2. Enter `secret_sauce` in the Password field.<br>3. Click the **Login** button. |
| Expected Result | The user remains on the login page and an error message is displayed. |
| Actual Result | The user remained on the login page and the following message was displayed: `Epic sadface: Username and password do not match any user in this service` |
| Status | Passed |

---

## TC-LOGIN-003 — Login attempt with an empty password

| Field | Details |
|---|---|
| Test Case ID | TC-LOGIN-003 |
| Title | Verify that login is rejected when the password field is empty |
| Priority | High |
| Preconditions | The Swag Labs login page is open |
| Test Data | Username: `standard_user` / Password: empty |
| Steps | 1. Enter `standard_user` in the Username field.<br>2. Leave the Password field empty.<br>3. Click the **Login** button. |
| Expected Result | The user remains on the login page and a password-required error message is displayed. |
| Actual Result | The user remained on the login page and the following message was displayed: `Epic sadface: Password is required` |
| Status | Passed |
