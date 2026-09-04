# FieldForceConnect QA Machine Test

Overview

This repository contains my QA Machine Test work for FieldForceConnect, covering Manual Testing, API Testing, and UI Automation.

---

1. Manual Testing

Manual testing was performed for the following modules:

- Sign Up
- Forgot Password
- Sign in with OTP
- Login

The manual testing workbook contains:

- Test Cases
- Field Validations
- Bugs

The identified application defect is documented in the Bugs sheet with steps, expected result, actual result, severity, priority, and evidence.

---

 2. API Testing - Postman

 Environment

- Environment: FieldForce Test
- Base URL: `https://test.fieldforceconnect.com`

 API Tests

Login - Valid Credentials

- Method: POST
- Endpoint: `/api/account/authenticate`
- Valid credentials were maintained using Postman environment variables.
- Response was verified successfully.

Login - Invalid Credentials

- Method: POST
- Endpoint: `/api/account/authenticate`
- Invalid credentials were used.
- Authentication error response was verified.

Add Customer

- Method: POST
- Endpoint: `/api/CRM/Lead`
- Authentication was configured for the request.
- Customer creation request was executed.
- Response and customer details were validated.

Postman Features Used

- Environment variables
- Base URL variable
- Authentication variables
- GET and POST requests
- Response validation
- Postman collection export

---

 3. UI Automation Testing

Technology Stack

- Java
- Maven
- Selenium WebDriver
- TestNG

Automation Scenarios

Login Journey

- Login flow automated using Selenium WebDriver.
- Test data is parameterized using TestNG DataProvider.
- Successful login and dashboard navigation are validated.

Punch In / Punch Out

- Attendance flow is automated through the UI.
- Punch In/Punch Out actions are covered where supported by the application.
- Toast/popup messages are captured and validated after the action.

Add Customer

- New Customer flow is automated.
- Customer test data is parameterized.
- Customer form fields are populated automatically.
- Save action is automated.
- Customer creation is validated after submission.

### Automation Structure

```text
fieldforceconnect-automation/
├── pom.xml
├── testng.xml
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   ├── pages/
│   │   │   └── utils/
│   │   └── resources/
│   └── test/
│       ├── java/
│       │   ├── base/
│       │   ├── pages/
│       │   └── tests/
│       └── resources/
