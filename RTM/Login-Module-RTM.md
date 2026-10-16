
# Login Module — Requirement Traceability Matrix (RTM)

## 1. Document Information

- **Project:** QA Portfolio Demonstration
- **Module:** Login / Authentication
- **Prepared By:** Mrunal Deshpande
- **Version:** 1.0
- **Status:** Sample — Requirements Not Yet Validated

## 2. Objective

The RTM maps sample login requirements to test cases
so that planned functionality can be traced to testing coverage.

The requirements below are illustrative and must be validated
against an actual specification before execution.

## 3. Requirement Traceability Matrix

| Requirement ID | Sample Requirement | Related Test Case IDs | Coverage Status |
|---|---|---|---|
| REQ_LOGIN_001 | Registered users can log in with valid credentials | TC_LOGIN_001 | Mapped |
| REQ_LOGIN_002 | Invalid credentials must not grant access | TC_LOGIN_002, TC_LOGIN_003 | Mapped |
| REQ_LOGIN_003 | Email and password are required | TC_LOGIN_004, TC_LOGIN_005, TC_LOGIN_006 | Mapped |
| REQ_LOGIN_004 | Email format is validated | TC_LOGIN_007 | Mapped |
| REQ_LOGIN_005 | Email whitespace is handled according to policy | TC_LOGIN_008 | Mapped |
| REQ_LOGIN_006 | Password comparison follows the authentication policy | TC_LOGIN_009 | Mapped |
| REQ_LOGIN_007 | Password visibility behaves correctly, if supported | TC_LOGIN_010 | Mapped |
| REQ_LOGIN_008 | Keyboard submission works, if supported | TC_LOGIN_011 | Mapped |
| REQ_LOGIN_009 | Repeated submissions are handled safely | TC_LOGIN_012 | Mapped |
| REQ_LOGIN_010 | Authentication resists injection attempts | TC_LOGIN_013, TC_LOGIN_014 | Mapped |
| REQ_LOGIN_011 | Long input is handled according to documented limits | TC_LOGIN_015, TC_LOGIN_016 | Mapped |
| REQ_LOGIN_012 | Email case handling follows the defined policy | TC_LOGIN_017 | Mapped |
| REQ_LOGIN_013 | Network failures are handled appropriately | TC_LOGIN_018 | Mapped |
| REQ_LOGIN_014 | Protected pages require valid authentication | TC_LOGIN_019 | Mapped |
| REQ_LOGIN_015 | Logout prevents unauthorized access to protected pages | TC_LOGIN_020 | Mapped |

## 4. Coverage Summary

- Sample requirements: 15
- Requirements mapped to test cases: 15
- Requirements without a mapped test case: 0
- Test execution status: Not executed

**Important:** Mapped coverage indicates that test cases
have been associated with sample requirements. It does not
prove that the requirements have been validated or passed.

## 5. Gaps and Follow-up

Confirm the following before execution:

- Password length and complexity requirements
- Account lockout and rate-limiting rules
- Required error messages
- Email normalization policy
- Session timeout and logout behavior
- Supported browsers and devices
- Multi-factor authentication requirements, if applicable

## 6. Conclusion

This RTM demonstrates how requirements can be linked
to test cases for traceability and coverage analysis.

Update the matrix when requirements or test cases change.
