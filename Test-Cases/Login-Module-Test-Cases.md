
# Login Module Test Cases

## Project Overview

- **Project:** QA Portfolio Demonstration
- **Module:** Login
- **Test Type:** Functional Testing
- **Status:** Test cases designed; execution pending

## Sample Requirement

Registered users can log in using their registered email address and password.

Successful authentication should allow access to the application. Invalid credentials must not grant access.

**Note:** Password rules, error messages, and account-lockout behavior must be confirmed against actual requirements.

## Test Cases

| Test Case ID | Scenario | Test Data / Steps | Expected Result | Priority |
|---|---|---|---|---|
| TC_LOGIN_001 | Login with valid credentials | Registered email + correct password | User logs in successfully | P1 |
| TC_LOGIN_002 | Incorrect password | Registered email + incorrect password | Login is rejected | P1 |
| TC_LOGIN_003 | Unregistered email | Unregistered email + password | Login is rejected | P1 |
| TC_LOGIN_004 | Empty email | Leave email blank; enter password | Required-field validation is shown, if specified | P1 |
| TC_LOGIN_005 | Empty password | Enter email; leave password blank | Required-field validation is shown, if specified | P1 |
| TC_LOGIN_006 | Both fields empty | Click Login without entering data | Login is prevented | P1 |
| TC_LOGIN_007 | Invalid email format | Enter `mrunal@` and a password | Invalid email is rejected | P1 |
| TC_LOGIN_008 | Email with surrounding spaces | Enter a valid email with spaces around it | Behavior matches email normalization requirements | P2 |
| TC_LOGIN_009 | Password case sensitivity | Change the case of a password character | Login is rejected if passwords are case-sensitive | P1 |
| TC_LOGIN_010 | Password visibility | Toggle the visibility control, if available | Password visibility changes correctly | P2 |
| TC_LOGIN_011 | Submit with Enter key | Enter credentials and press Enter | Form submits if keyboard submission is supported | P2 |
| TC_LOGIN_012 | Rapid repeated clicks | Click Login several times quickly | No duplicate or inconsistent processing | P2 |
| TC_LOGIN_013 | SQL injection-like input | Enter a safe test string such as `' OR '1'='1` | Authentication is not bypassed | P1 |
| TC_LOGIN_014 | Script-like input | Enter `<script>alert(1)</script>` as input | Input is handled safely without script execution | P1 |
| TC_LOGIN_015 | Very long email | Enter an unusually long email value | Input is handled according to documented limits | P2 |
| TC_LOGIN_016 | Very long password | Enter a long password value | Input is handled securely and consistently | P2 |
| TC_LOGIN_017 | Email case variation | Change the case of a registered email | Behavior follows the documented email policy | P2 |
| TC_LOGIN_018 | Network interruption | Interrupt the network during login | An appropriate error appears; no false success occurs | P2 |
| TC_LOGIN_019 | Protected page after login | Log in and open a protected page | Access follows the session policy | P1 |
| TC_LOGIN_020 | Protected page after logout | Log out and revisit a protected page | Access is denied or redirected according to policy | P1 |

## Test Execution Summary

- Total test cases: 20
- Passed: 0
- Failed: 0
- Blocked: 0
- Not Run: 20

**Execution status:** Not executed. These are designed test cases, not verified test results.

## Open Questions

1. What are the password length and complexity requirements?
2. Is there an account-lockout or rate-limiting policy?
3. What messages should appear for invalid credentials?
4. Is multi-factor authentication required?
5. What are the session timeout requirements?

## Conclusion

These test cases demonstrate a structured approach to login testing, including positive, negative, boundary, security-oriented, and session-related scenarios.

Actual results should be recorded only after execution against an identified application version.
