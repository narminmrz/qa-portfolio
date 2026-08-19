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
