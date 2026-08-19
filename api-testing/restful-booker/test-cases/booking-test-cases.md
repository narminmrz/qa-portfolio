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
