# Safe API Security Test Matrix

Use only a controlled lab or explicitly authorized target. Create synthetic accounts A and B and synthetic objects.

| ID | Risk | Safe test | Expected secure behavior |
|---|---|---|---|
| SEC-001 | BOLA | User B requests User A's synthetic object | Access denied or safely concealed |
| SEC-002 | Authentication | Call protected route without token | 401; no protected data |
| SEC-003 | Token validation | Use expired or malformed test token | Request rejected |
| SEC-004 | Function authorization | Low-privilege role calls admin route | 403 or documented denial |
| SEC-005 | Property authorization | Attempt to change protected synthetic field | Field rejected or ignored |
| SEC-006 | Excessive data exposure | Inspect low-privilege response fields | Only authorized fields returned |
| SEC-007 | Rate limiting | Small pre-approved request sequence | Documented throttling enforced |
| SEC-008 | Input validation | Submit malformed types to lab endpoint | Safe validation error |
| SEC-009 | Misconfiguration | Review headers and error messages | No secrets or internals exposed |
| SEC-010 | Inventory | Compare documented and approved deployed routes | Deprecated versions controlled |
| SEC-011 | SSRF | Test URL-fetch feature against local mock | Internal/restricted destinations blocked |
| SEC-012 | Third-party trust | Feed invalid upstream data to mock | Upstream data validated |

Never enumerate or access real users' objects. Stop if unexpected data is returned.
