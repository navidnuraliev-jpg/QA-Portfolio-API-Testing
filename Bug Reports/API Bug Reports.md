# API Bug Reports

## BUG-001 - POST request accepts empty title (Demo)

**Environment**
- Postman v11
- JSONPlaceholder API

**Method**
POST

**Endpoint**
/posts

**Severity**
Medium

**Priority**
Medium

**Status**
Open

**Preconditions**
API is available.

**Steps to Reproduce**
1. Send POST request.
2. Leave the `title` field empty.
3. Submit the request.

**Expected Result**
API should return validation error (400 Bad Request).

**Actual Result**
API accepts the request and returns **201 Created**.

---

## BUG-002 - Invalid endpoint returns unclear response (Demo)

**Environment**
- Postman v11
- JSONPlaceholder API

**Method**
GET

**Endpoint**
/postssss

**Severity**
Low

**Priority**
Low

**Status**
Open

**Preconditions**
API is available.

**Steps to Reproduce**
1. Send GET request to `/postssss`.

**Expected Result**
API returns a clear error message explaining that the endpoint does not exist.

**Actual Result**
API returns a generic 404 response without detailed information.

---

## BUG-003 - Missing validation for negative userId (Demo)

**Environment**
- Postman v11
- JSONPlaceholder API

**Method**
POST

**Endpoint**
/posts

**Severity**
Medium

**Priority**
Low

**Status**
Open

**Preconditions**
API is available.

**Steps to Reproduce**
1. Send POST request.
2. Set `"userId": -1`.
3. Submit the request.

**Expected Result**
API should reject invalid userId.

**Actual Result**
Request is accepted successfully.

---

## Note

JSONPlaceholder is a public fake REST API used for learning and testing purposes. The bug reports above are demonstration examples created to showcase API bug reporting skills.
