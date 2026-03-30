# Requirement Traceability Matrix (RTM)
RTM (Requirement Traceability Matrix) is a document or table that links requirements to test scenarios and test cases.

✅ Purpose:
Ensures every requirement is tested.
Provides traceability: You can track each requirement from design → testing → closure.
Helps QA identify missing test cases or untested requirements.
Useful for audits, sign-offs, and project tracking.

🔹 Key Features:
## Feature	Description
1. Traceability	Maps requirements → test scenarios → test cases → test execution status
2. Coverage	Confirms that all functional/non-functional requirements are covered
3. Tracking	Shows which requirements are done, in progress, or not tested
4. Documentation	Serves as proof for QA coverage for stakeholders

| Req_ID | Requirement Description | Test Scenario | Test Case | Status |
|--------|------------------------|---------------|-----------|--------|
| RQ_01 | User should login with valid credentials | Login with valid credentials | TC_01 | Covered |
| RQ_02 | User should see error on invalid login | Login with invalid credentials | TC_02 | Covered |
| RQ_03 | User can add items to cart | Add product to cart | TC_01 (Cart) | Covered |
| RQ_04 | Cart should update quantity and total | Update quantity | TC_03 (Cart) | Covered |
| RQ_05 | User can complete checkout | Submit checkout with valid data | TC_01 (Checkout) | Covered |
