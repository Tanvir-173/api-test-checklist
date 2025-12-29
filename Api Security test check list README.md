# API Security Test Checklist

This document provides a comprehensive checklist for **API Security Testing** based on industry best practices and **OWASP API Security Top 10** guidelines.  
It is intended for **QA Engineers, Automation Testers, Security Testers, and Developers** to ensure APIs are secure, reliable, and resilient against attacks.

---

##  Purpose
The purpose of this checklist is to:
- Identify security vulnerabilities in APIs
- Prevent unauthorized access and data exposure
- Ensure compliance with security standards
- Strengthen authentication, authorization, and data protection

---

##  1. Authentication
- API enforces authentication where required
- Valid credentials/token allow access
- Invalid or missing credentials are rejected
- Expired tokens are rejected
- Token refresh mechanism works correctly
- No default or hardcoded credentials

---

##  2. Authorization (Access Control)
- Role-based access control (RBAC) enforced
- Users cannot access other users’ data (BOLA check)
- Admin endpoints are properly restricted
- Privilege escalation is not possible
- Permissions validated for every request

---

##  3. Token & Session Security
- Tokens are securely generated and signed
- Token expiration time enforced
- Token scopes validated
- Tokens not exposed in URLs or logs
- Tokens invalidated on logout or expiry

---

##  4. Input Validation & Injection Protection
- SQL Injection attacks prevented
- NoSQL Injection attacks prevented
- Command Injection prevented
- Cross-Site Scripting (XSS) payloads rejected
- Input data sanitized and validated

---

##  5. Transport Security
- HTTPS enforced for all endpoints
- Valid TLS/SSL certificates
- Weak ciphers disabled
- Secure headers applied (if applicable)

---

##  6. Rate Limiting & Throttling
- Rate limiting implemented per user/IP
- Excessive requests blocked with HTTP 429
- Brute-force protection enabled
- API abuse detection in place

---

##  7. Data Exposure & Privacy
- No sensitive data exposed in responses
- Personally Identifiable Information (PII) masked or omitted
- Error messages do not reveal system details
- Stack traces hidden in production
- Pagination enforced to avoid data dumps

---

##  8. HTTP Method & CORS Security
- Only allowed HTTP methods enabled
- Unsupported methods blocked (405 Method Not Allowed)
- OPTIONS method restricted if not required
- Proper CORS policy configured

---

##  9. Business Logic Security
- Workflow sequence enforced
- Duplicate or replay attacks prevented
- Race conditions handled
- Limits enforced (transaction limits, retry limits)

---

##  10. File & Payload Security
- File type validation enforced
- File size limits applied
- Malware scanning (if applicable)
- JSON/XML schema validation
- XML External Entity (XXE) attacks prevented

---

##  11. Logging & Monitoring
- Security-related events logged
- Failed authentication attempts logged
- No sensitive data stored in logs
- Alerts enabled for suspicious activities

---

##  12. OWASP API Security Top 10 Coverage
- Broken Object Level Authorization (BOLA)
- Broken User Authentication
- Excessive Data Exposure
- Lack of Rate Limiting
- Mass Assignment
- Security Misconfiguration
- Injection
- Improper Asset Management
- Insufficient Logging & Monitoring
- Server-Side Request Forgery (SSRF)

---

##  Tools (Optional)
- Postman / Newman
- OWASP ZAP / Burp Suite
- Swagger / OpenAPI
- Playwright API / Rest Assured
- JMeter / k6 for security performance

---

##  Conclusion
Following this API Security Test Checklist helps ensure APIs are protected against common vulnerabilities, unauthorized access, and data leaks while maintaining compliance with security best practices.

---

