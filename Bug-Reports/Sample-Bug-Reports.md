Sample Bug Reports

Project Information
- Project: Login Module — Portfolio Demonstration
- Module:Authentication
- **Environment: Hypothetical test environment
- **Status:** Sample reports; not verified against a live application

## BUG-001: Login Does Not Reject Invalid Credentials

**Severity:** High — proposed  
**Priority:** P1 — proposed  
**Status:** Not Verified

### Preconditions
A test account exists in an authorized test environment.

### Steps to Reproduce
1. Open the login page.
2. Enter a registered email address.
3. Enter an incorrect password.
4. Click Login.

### Expected Result
The application rejects authentication and does not grant access to protected pages.

### Actual Result
Not tested. Record the observed behavior after reproducing the issue.

### Evidence
To be added after verification.

---

## BUG-002: Required Field Validation Is Missing

**Severity:** Medium — proposed  
**Priority:** P2 — proposed  
**Status:** Not Verified

### Steps to Reproduce
1. Open the login page.
2. Leave the email field empty.
3. Enter a password.
4. Click Login.

### Expected Result
The application displays appropriate validation and prevents invalid submission, according to requirements.

### Actual Result
Not tested.

### Evidence
To be added after verification.

---

## BUG REPORTING CHECKLIST

- Unique defect ID
- Clear title and description
- Preconditions and reproducible steps
- Expected and actual results
- Environment and evidence
- Severity, priority, and status

**Note:** These are illustrative examples, not verified defects. Confirm actual behavior before reporting a real bug.

