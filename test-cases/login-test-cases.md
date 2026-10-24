# Login Test Cases

## 1. Overview

- **Application:** Sample Telecom Mobile App
- **Feature:** User Login
- **Platforms:** iOS and Android
- **Testing types:** Functional, positive, negative, and boundary value testing

## 2. Preconditions

- The application is installed and launched.
- An authorised test account is available.
- The test environment is accessible.

## 3. Test Cases

### LOGIN_001: Login with Valid Credentials

**Priority:** High

**Test Steps:**
1. Open the application.
2. Enter valid login credentials.
3. Tap the Login button.

**Test Data:** Valid test account

**Expected Result:** The user logs in successfully and reaches the home screen.

---

### LOGIN_002: Login with an Incorrect Password

**Priority:** High

**Test Steps:**
1. Open the login screen.
2. Enter a registered account and an incorrect password.
3. Tap the Login button.

**Test Data:** Registered test account with an incorrect password

**Expected Result:** Login is rejected and an appropriate error message is displayed.

---

### LOGIN_003: Login with an Unregistered Account

**Priority:** High

**Test Steps:**
1. Open the login screen.
2. Enter unregistered account details.
3. Tap the Login button.

**Test Data:** Unregistered test account

**Expected Result:** Login is rejected and access is not granted.

---

### LOGIN_004: Submit with Empty Fields

**Priority:** High

**Test Steps:**
1. Open the login screen.
2. Leave the required fields empty.
3. Tap the Login button.

**Test Data:** Blank username and password fields

**Expected Result:** Required-field validation is displayed and login does not proceed.

---

### LOGIN_005: Verify Password Masking

**Priority:** Medium

**Test Steps:**
1. Open the login screen.
2. Enter a password.

**Test Data:** Sample test password

**Expected Result:** Password characters are masked by default.

---

### LOGIN_006: Login When the Network Is Disconnected

**Priority:** High

**Test Steps:**
1. Disable the device's network connection.
2. Enter valid login credentials.
3. Tap the Login button.

**Test Data:** Valid test account; network disconnected

**Expected Result:** The application handles the connection failure gracefully and displays an appropriate message.

---

### LOGIN_007: Verify Password Length Boundaries

**Priority:** Medium

**Test Steps:**
1. Check the documented minimum and maximum password lengths.
2. Enter passwords at the boundary lengths.
3. Attempt to log in.

**Test Data:** Passwords matching the documented boundary lengths

**Expected Result:** The application accepts or rejects password lengths according to the defined requirements.

## 4. Notes

- Use only fictional or authorised test accounts.
- Confirm expected behaviour against approved requirements.
- Password length rules and error messages may vary by application.
