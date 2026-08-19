# Restful Booker — Booking API Test Cases

## TC-API-001 — Get all booking IDs

| Field | Details |
|---|---|
| Test Case ID | TC-API-001 |
| Title | Verify that the API returns a list of booking IDs |
| Method | `GET` |
| Endpoint | `/booking` |
| Priority | High |
| Preconditions | The Restful Booker API is available |
| Steps | 1. Send a `GET` request to `https://restful-booker.herokuapp.com/booking`. |
| Expected Result | The API returns status code `200 OK` and a JSON array containing `bookingid` values. |
| Actual Result | The API returned status code `200 OK` and a JSON array containing `bookingid` values. |
| Status | Passed |


---

## TC-API-002 — Get booking details by ID

| Field | Details |
|---|---|
| Test Case ID | TC-API-002 |
| Title | Verify that the API returns booking details for a valid booking ID |
| Method | `GET` |
| Endpoint | `/booking/3` |
| Priority | High |
| Preconditions | Booking ID `3` exists |
| Steps | 1. Send a `GET` request to `https://restful-booker.herokuapp.com/booking/3`. |
| Expected Result | The API returns status code `200 OK` and booking details containing `firstname`, `lastname`, `totalprice`, and `bookingdates`. |
| Actual Result | The API returned status code `200 OK` and booking details containing the expected fields. |
| Status | Passed |


---

## TC-API-003 — Get booking details with a non-existent ID

| Field | Details |
|---|---|
| Test Case ID | TC-API-003 |
| Title | Verify that the API returns `404 Not Found` for a non-existent booking ID |
| Method | `GET` |
| Endpoint | `/booking/99999999` |
| Priority | Medium |
| Preconditions | The Restful Booker API is available |
| Steps | 1. Send a `GET` request to `https://restful-booker.herokuapp.com/booking/99999999`. |
| Expected Result | The API returns status code `404 Not Found` and response text `Not Found`. |
| Actual Result | The API returned status code `404 Not Found` and response text `Not Found`. |
| Status | Passed |


---

## TC-API-004 — Create a new booking

| Field | Details |
|---|---|
| Test Case ID | TC-API-004 |
| Title | Verify that the API creates a booking with valid data |
| Method | `POST` |
| Endpoint | `/booking` |
| Priority | High |
| Preconditions | The Restful Booker API is available |
| Request Body | `{"firstname":"QA","lastname":"Portfolio","totalprice":150,"depositpaid":true,"bookingdates":{"checkin":"2026-09-10","checkout":"2026-09-15"},"additionalneeds":"Breakfast"}` |
| Steps | 1. Send a `POST` request to `https://restful-booker.herokuapp.com/booking` with valid booking data. |
| Expected Result | The API returns status code `200 OK` and a response containing a new `bookingid`. |
| Actual Result | The API created a new booking and returned `bookingid: 1452`. |
| Status | Passed |

---

## TC-API-005 — Get the newly created booking

| Field | Details |
|---|---|
| Test Case ID | TC-API-005 |
| Title | Verify that the newly created booking can be retrieved |
| Method | `GET` |
| Endpoint | `/booking/1452` |
| Priority | High |
| Preconditions | Booking ID `1452` was created successfully |
| Steps | 1. Send a `GET` request to `https://restful-booker.herokuapp.com/booking/1452`. |
| Expected Result | The API returns status code `200 OK` and booking details with firstname `QA` and lastname `Portfolio`. |
| Actual Result | The API returned status code `200 OK` and displayed firstname `QA` and lastname `Portfolio`. |
| Status | Passed |
