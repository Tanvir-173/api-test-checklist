# API Test Checklist

This document provides a comprehensive checklist for **API Testing**.  
It is intended for **QA Engineers, Automation Testers, and Developers** to ensure APIs are reliable, secure, and meet business requirements.

---

##  Purpose
The purpose of this checklist is to:
- Validate API functionality and data integrity
- Ensure correct request and response handling
- Detect defects early in the development cycle
- Support manual and automated API testing

---

##  1. API Basics & Contract Validation
- Correct API endpoint URL
- Correct HTTP method (GET, POST, PUT, PATCH, DELETE)
- API versioning handled correctly
- Required headers provided (Content-Type, Authorization)
- Request body matches API contract

---

##  2. Request Validation
- Valid requests return successful responses
- Missing mandatory parameters handled properly
- Invalid parameters return appropriate errors
- Data types and formats validated
- Boundary values tested
- Empty request body handled correctly

---

##  3. Response Validation
- Correct HTTP status codes returned
- Response time within acceptable limits
- Response body matches defined schema
- Data types in response are correct
- Response headers validated
- No sensitive data exposed in response

---

##  4. Authentication & Authorization
- Authenticated requests allowed
- Unauthenticated requests rejected
- Invalid or expired tokens handled correctly
- Role-based access control validated
- Unauthorized data access prevented

---

##  5. CRUD Operations
- Create operations work correctly
- Read operations return correct data
- Update operations modify data accurately
- Delete operations remove or deactivate data properly
- Data consistency maintained across operations

---

##  6. Business Logic Validation
- Business rules enforced correctly
- Workflow sequences validated
- Duplicate requests handled properly
- Correct error messages for business rule violations

---

##  7. Performance & Reliability
- API response time within SLA
- Handles concurrent requests correctly
- No unexpected timeouts
- Rate limiting behavior validated

---

##  8. Error Handling & Negative Testing
- Meaningful error messages returned
- Proper HTTP error codes used
- Graceful handling of server errors
- No stack traces exposed

---

##  9. Idempotency & Retry
- GET requests are idempotent
- Retry-safe operations validated
- Duplicate request handling verified
- Idempotency keys supported where applicable

---

##  10. Security (Basic API Level)
- HTTPS enforced
- Input validation prevents injection attacks
- Sensitive data not logged or exposed
- CORS policy validated

---

##  11. Documentation & Versioning
- API documentation matches actual behavior
- Swagger / OpenAPI definitions up to date
- Deprecated endpoints handled properly
- Backward compatibility maintained

---

##  Tools (Optional)
- Postman / Newman
- Swagger / OpenAPI
- Playwright API / Rest Assured
- JMeter / k6

---

##  Conclusion
Following this API Test Checklist ensures APIs are robust, reliable, and aligned with functional and business requirements.

---

