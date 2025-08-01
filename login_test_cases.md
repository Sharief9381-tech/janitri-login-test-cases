# Test Cases for Janitri Dashboard Login Page

**URL**: https://dev-dash.janitri.in

## Test Case Structure
- **Test Case ID**: Unique identifier
- **Test Scenario**: Description of what is being tested
- **Preconditions**: Requirements before testing
- **Test Steps**: Steps to execute
- **Expected Result**: Anticipated outcome
- **Test Type**: Positive or Negative

## Positive Test Cases

### TC_Login_001: Successful Login with Valid Email and Password
- **Test Scenario**: Verify that a user can log in with valid credentials.
- **Preconditions**: User has a registered account.
- **Test Steps**:
  1. Navigate to https://dev-dash.janitri.in.
  2. Enter valid email (e.g., testuser@janitri.in).
  3. Enter correct password (e.g., Password123!).
  4. Click "Login".
- **Expected Result**: User is redirected to the dashboard.
- **Test Type**: Positive

### TC_Login_002: Successful Login with "Remember Me" Enabled
- **Test Scenario**: Verify that enabling "Remember Me" retains login session.
- **Preconditions**: "Remember Me" option is available.
- **Test Steps**:
  1. Navigate to https://dev-dash.janitri.in.
  2. Enter valid credentials.
  3. Check "Remember Me".
  4. Click "Login".
  5. Log out and revisit the page.
- **Expected Result**: User remains logged in or credentials are pre-filled.
- **Test Type**: Positive

## Negative Test Cases

### TC_Login_003: Login with Invalid Email
- **Test Scenario**: Verify behavior with an invalid email.
- **Preconditions**: None.
- **Test Steps**:
  1. Navigate to https://dev-dash.janitri.in.
  2. Enter invalid email (e.g., nonexist@janitri.in).
  3. Enter a password.
  4. Click "Login".
- **Expected Result**: Error: "Invalid email or password."
- **Test Type**: Negative

### TC_Login_004: Login with Empty Fields
- **Test Scenario**: Verify behavior when both fields are empty.
- **Preconditions**: None.
- **Test Steps**:
  1. Navigate to https://dev-dash.janitri.in.
  2. Leave email and password blank.
  3. Click "Login".
- **Expected Result**: Errors: "Email is required" and "Password is required."
- **Test Type**: Negative