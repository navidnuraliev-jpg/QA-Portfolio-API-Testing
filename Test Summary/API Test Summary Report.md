# API Test Summary Report

## Project

JSONPlaceholder REST API

---

## Test Objective

Verify the basic functionality of the JSONPlaceholder REST API using Postman.

---

## Test Environment

- Postman v11
- JSONPlaceholder REST API
- Windows 11
- HTTPS

---

## Tested Endpoints

| Method | Endpoint | Status |
|---------|----------|--------|
| GET | /posts/1 | Passed |
| GET | /posts | Passed |
| POST | /posts | Passed |
| PUT | /posts/1 | Passed |
| PATCH | /posts/1 | Passed |
| DELETE | /posts/1 | Passed |

---

## Test Metrics

| Metric | Value |
|--------|-------|
| Total Test Cases | 6 |
| Passed | 6 |
| Failed | 0 |
| Blocked | 0 |
| Pass Rate | 100% |

---

## API Validations Performed

- Status code validation
- Response body validation
- JSON schema structure verification
- Response time validation
- Content-Type validation
- Data consistency verification

---

## Defects

No functional defects were found during testing.

The demonstration bug reports included in this repository were created for portfolio purposes only because JSONPlaceholder is a public fake REST API.

---

## Release Recommendation

The tested API endpoints meet the expected behavior and are recommended for release.

---

## Conclusion

The API successfully handled all tested requests.

The Postman collection contains automated validation scripts for every request, making it suitable for future regression testing and API automation practice.
