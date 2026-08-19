# OrangeHRM — Login Test Cases

## TC-LOGIN-001 — Successful login with valid credentials

| Field | Details |
|---|---|
| Test Case ID | TC-LOGIN-001 |
| Title | Verify that an admin user can log in with valid credentials |
| Priority | High |
| Preconditions | The OrangeHRM login page is open |
| Test Data | Username: `Admin` / Password: `admin123` |
| Steps | 1. Enter `Admin` in the Username field.<br>2. Enter `admin123` in the Password field.<br>3. Click **Login**. |
| Expected Result | The user is redirected to the Dashboard and the navigation menu is displayed. |
| Actual Result | The user was redirected to the Dashboard and the navigation menu was displayed. |
| Status | Passed |


---

## TC-LOGIN-002 — Login attempt with an invalid username

| Field | Details |
|---|---|
| Test Case ID | TC-LOGIN-002 |
| Title | Verify that login is rejected when an invalid username is entered |
| Priority | High |
| Preconditions | The OrangeHRM login page is open |
| Test Data | Username: `wrong_user` / Password: `admin123` |
| Steps | 1. Enter `wrong_user` in the Username field.<br>2. Enter `admin123` in the Password field.<br>3. Click **Login**. |
| Expected Result | The user remains on the login page and an invalid credentials message is displayed. |

---

## TC-LOGIN-003 — Login attempt with an empty username

| Field | Details |
|---|---|
| Test Case ID | TC-LOGIN-003 |
| Title | Verify validation when the Username field is empty |
| Priority | High |
| Preconditions | The OrangeHRM login page is open |
| Test Data | Username: empty / Password: `admin123` |
| Steps | 1. Leave the Username field empty.<br>2. Enter `admin123` in the Password field.<br>3. Click **Login**. |
| Expected Result | The user remains on the login page and a `Required` validation message is displayed below the Username field. |
| Actual Result | The user remained on the login page. A `Required` validation message was displayed below the Username field, and `Invalid credentials` was also displayed. |
| Status | Passed |
| Actual Result | The user remained on the login page and the following message was displayed: `Invalid credentials` |
| Status | Passed |
