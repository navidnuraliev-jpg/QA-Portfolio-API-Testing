# API Test Cases

## TC-001 - Get a single post by valid ID

**Method:** GET

**Endpoint:** /posts/1

**Preconditions**
- API server is available.

**Steps**
1. Send GET request to `/posts/1`.

**Expected Result**
- Status code is **200 OK**.
- Response body is JSON.
- Response contains:
  - id = 1
  - userId
  - title
  - body.

---

## TC-002 - Get all posts

**Method:** GET

**Endpoint:** /posts

**Preconditions**
- API server is available.

**Steps**
1. Send GET request to `/posts`.

**Expected Result**
- Status code is **200 OK**.
- Response is an array.
- Array is not empty.
- Each object contains:
  - id
  - userId
  - title
  - body.

---

## TC-003 - Create a new post

**Method:** POST

**Endpoint:** /posts

**Request Body**

```json
{
  "title": "QA Portfolio Test",
  "body": "Created using Postman",
  "userId": 1
}
```

**Steps**
1. Send POST request.

**Expected Result**
- Status code is **201 Created**.
- Response contains generated **id**.
- Returned title matches request.
- Returned body matches request.
- Returned userId equals **1**.

---

## TC-004 - Update existing post

**Method:** PUT

**Endpoint:** /posts/1

**Steps**
1. Send PUT request with updated data.

**Expected Result**
- Status code is **200 OK**.
- Response contains updated values.
- Response contains id = 1.

---

## TC-005 - Partially update a post

**Method:** PATCH

**Endpoint:** /posts/1

**Steps**
1. Update only the title.

**Expected Result**
- Status code is **200 OK**.
- Title is updated.
- Other fields remain unchanged.

---

## TC-006 - Delete a post

**Method:** DELETE

**Endpoint:** /posts/1

**Steps**
1. Send DELETE request.

**Expected Result**
- Status code is **200 OK**.
- Request is processed successfully.
