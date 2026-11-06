# API Security Assessment Methodology

## 1. Authorization and scope
Record system owner, written permission, approved domains/IPs, endpoints, test window, allowed techniques, prohibited actions, emergency contact, and evidence-retention rules.

## 2. Understand the API
Review documentation, versions, endpoints, roles, data classification, authentication model, and trust boundaries.

## 3. Establish a baseline
Use a low-privilege synthetic account. Record method, endpoint, role, status, and response fields with tokens redacted.

## 4. Validate controls
Check authentication, object ownership, function permissions, property-level access, input validation, rate limits, and error handling. Use synthetic records only.

## 5. Report findings
Include preconditions, minimal reproduction steps, expected versus actual behavior, impact, severity rationale, and remediation. Avoid retaining sensitive response bodies.

## 6. Retest
Retest only with permission and record the fixed build, date, result, and residual risk.
