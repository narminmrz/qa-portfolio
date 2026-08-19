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


---

## TC-AUTH-002 — Authentication attempt with invalid credentials

| Field | Details |
|---|---|
| Test Case ID | TC-AUTH-002 |
| Title | Verify that the API rejects invalid authentication credentials |
| Method | `POST` |
| Endpoint | `/auth` |
| Priority | High |
| Preconditions | The Restful Booker API is available |
| Request Body | `{"username": "admin", "password": "wrong_password"}` |
| Steps | 1. Send a `POST` request to `https://restful-booker.herokuapp.com/auth` with an invalid password. |
| Expected Result | The API returns status code `200 OK` and a response containing `{"reason": "Bad credentials"}`. |
| Actual Result | The API returned status code `200 OK` and response `{"reason": "Bad credentials"}`. |
| Status | Passed |
