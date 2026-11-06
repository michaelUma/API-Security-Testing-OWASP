# API Security Testing — OWASP

An authorization-first portfolio demonstrating how API security risks are translated into safe test cases, evidence, and remediation advice.

## Reference
OWASP API Security Top 10 (2023): https://owasp.org/API-Security/

## Coverage
- Broken Object Level Authorization (BOLA)
- Broken Authentication
- Broken Object Property Level Authorization
- Unrestricted Resource Consumption
- Broken Function Level Authorization
- Sensitive Business Flow Abuse
- Server-Side Request Forgery (SSRF)
- Security Misconfiguration
- Improper Inventory Management
- Unsafe Consumption of APIs

## Repository map
- `docs/METHODOLOGY.md` — authorized assessment workflow
- `test-cases/SECURITY-TEST-CASES.md` — safe security matrix
- `checklists/ENGAGEMENT-CHECKLIST.md` — authorization checklist
- `reports/FINDING-TEMPLATE.md` — report format

## Safe workflow
1. Obtain written permission and define exact scope.
2. Use a dedicated lab, synthetic accounts, and synthetic records.
3. Establish a normal-request baseline.
4. Test one security control at a time.
5. Stop if real user data or service impact is encountered.
6. Store only minimal sanitized evidence.
7. Explain impact, remediation, and retest outcome.

## Tools
Postman, curl, browser developer tools, and an intercepting proxy can support authorized testing. Tool access does not equal authorization.

## Safety boundary
Do not test third-party or production systems without explicit permission. Avoid denial-of-service, credential attacks, destructive actions, and data extraction. Use intentionally vulnerable local labs for exploit practice.

## Evidence integrity
The repository provides a methodology and test templates; it does not claim that a live security assessment has been performed.

## Author
Michael Uma — API Security Testing Portfolio.
