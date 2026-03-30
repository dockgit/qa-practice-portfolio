# API Testing

## What is API Testing?
API Testing is a type of testing where application programming interfaces are tested directly to ensure functionality, reliability, and security.
API Testing focuses on validating the business logic layer (between frontend & database).
---
Instead of UI clicks, QA sends HTTP requests and verifies:

Response data
Status codes
Performance
Security

👉 You are testing contract between client ↔ server
----

🔹 How QA Actually Performs API Testing (Step-by-Step)

✅ Step 1: Understand API Documentation
## Sources:
Swagger
Postman Collection
Dev docs

## You identify:
Endpoint (URL)
Method (GET, POST, etc.)
Request body
Headers
Expected response

✅ Step 2: Prepare Test Scenarios
## Example (Login API):
Valid login
Invalid password
Missing fields
SQL injection attempt
Empty request

✅ Step 3: Create Test Cases
## Example:
Test Case	Input	Expected Output
Valid Login	correct email/pass	-- 200 + token
Wrong Pass	valid email, wrong pass	-- 401 error
Empty Fields	null	-- validation error

✅ Step 4: Send Requests (Using Tools)
## Tools:
Postman (most common)
Swagger UI
Curl (CLI)
Automation: Jest / Supertest / Newman
----
🔹 Example API Testing (Real)
## POST /login
Request:
{
  "email": "test@gmail.com",
  "password": "123456"
}

## Expected Response:
{
  "token": "abc123",
  "user": {
    "id": 1,
    "email": "test@gmail.com"
  }
}

----
## Why API Testing?
- Faster than UI testing
- Detects early bugs
- Independent of frontend

## Tools Used
- Postman
- Swagger

## Types of API Testing
- Functional Testing  (API works correctly)
- Load Testing   (check 'Input validation', 'Required Field')
- Security Testing  (check 'Authentication', 'Authorization')
- Load Testing (check API under heavy traffic)  Tools | JMeter, k6

## HTTP Methods
- GET → Fetch data
- POST → Create data
- PUT → Update data
- DELETE → Remove data
