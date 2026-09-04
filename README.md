# Automation Exercise API Testing Project

## Project Overview

This project contains REST API testing performed on the Automation Exercise e-commerce application using Postman.

The purpose of this project is to validate API functionality, response data, error handling, and user account operations through positive and negative test scenarios.

---

## Tools Used

- Postman
- JavaScript (Postman Test Scripts)
- Jira (Test Management & Bug Tracking)
- GitHub

---

## API Test Coverage

| Test ID | API Scenario | Method | Status |
|---|---|---|---|
| API_001 | Get All Products List | GET | ✅ PASS |
| API_002 | POST To All Products List | POST | ✅ PASS |
| API_003 | Get All Brands List | GET | ✅ PASS |
| API_004 | PUT To All Brands List | PUT | ✅ PASS |
| API_005 | Search Product | POST | ✅ PASS |
| API_006 | Search Product Without Parameter | POST | ✅ PASS |
| API_007 | Login With Valid Details | POST | ✅ PASS |
| API_008 | Login Without Email Parameter | POST | ✅ PASS |
| API_009 | DELETE Verify Login | DELETE | ✅ PASS |
| API_010 | Login With Invalid Details | POST | ✅ PASS |
| API_011 | Create/Register User Account | POST | ✅ PASS |
| API_012 | Delete User Account | DELETE | ✅ PASS |
| API_013 | Update User Account | PUT | ✅ PASS |
| API_014 | Get User Account Detail By Email | GET | ✅ PASS |

---

## Testing Activities Performed

### API Functional Testing
- Verified API endpoints
- Tested different HTTP methods:
  - GET
  - POST
  - PUT
  - DELETE

### Response Validation
Validated:

- HTTP status codes
- API response codes
- Response messages
- JSON response structure
- Required fields

### Positive Testing

Examples:
- Successful user login
- Product search
- User registration
- User update
- Account deletion
- User details retrieval

### Negative Testing

Examples:
- Login with invalid credentials
- Missing required parameters
- Unsupported HTTP methods
- Duplicate email registration

---

## Postman Test Automation

JavaScript assertions were created in Postman to automate validation.

Example:

```javascript
pm.test("Status code should be 200", function () {
    pm.response.to.have.status(200);
});
## Test Execution Evidence

Screenshots from Postman execution:

| API | Evidence |
|---|---|
| API_001 Get All Products List | Screenshot available |
| API_002 POST All Products List | Screenshot available |
| API_003 Get All Brands List | Screenshot available |
| API_004 PUT All Brands List | Screenshot available |
| API_005 Search Product | Screenshot available |
| API_006 Search Product Without Parameter | Screenshot available |
| API_007 Login With Valid Details | Screenshot available |
| API_008 Login Without Email Parameter | Screenshot available |
| API_009 DELETE Verify Login | Screenshot available |
| API_010 Login With Invalid Details | Screenshot available |
| API_011 Create User Account | Screenshot available |
| API_012 Delete User Account | Screenshot available |
| API_013 Update User Account | Screenshot available |
| API_014 Get User Details | Screenshot available |

## Jira Test Management Evidence

Jira was used to manage testing activities, track defects, and document API testing tasks.

Evidence includes:

- Jira project workflow board
- API testing task management
- Bug reporting with severity and priority
- Test execution tracking

Tools:
- Jira
- Postman
- GitHub
