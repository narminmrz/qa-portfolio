# Restful Booker — Authentication API Test Cases

## TC-AUTH-001 — Create an authentication token with valid credentials

| Field | Details |
|---|---|
| Test Case ID | TC-AUTH-001 |
| Title | Verify that the API creates an authentication token with valid credentials |
| Method | `POST` |
| Endpoint | `/auth` |
| Priority | High |
| Preconditions | The Restful Booker API is available |
| Request Body | `{"username": "admin", "password": "password123"}` |
| Steps | 1. Send a `POST` request to `https://restful-booker.herokuapp.com/auth` with valid credentials. |
| Expected Result | The API returns status code `200 OK` and a response containing a `token`. |
| Actual Result | The API returned status code `200 OK` and a response containing a `token`. |
| Status | Passed |
