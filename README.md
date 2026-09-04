# FieldForceConnect QA Machine Test

 Overview

This repository contains my QA Machine Test work for FieldForceConnect, covering Manual Testing, API Testing, and UI Automation.

 1. Postman API Testing

 Environment

- Environment: FieldForce Test
- Base URL: https://test.fieldforceconnect.com

 API Tests Performed

 Login - Valid Credentials
- Method: POST
- Endpoint: `/api/account/authenticate`
- Valid credentials were used through Postman environment variables.
- Response was verified successfully.

 Login - Invalid Credentials
- Method: POST
- Endpoint: `/api/account/authenticate`
- Invalid password was used.
- Response was verified with an authentication error message.

 Add Customer
- Method: POST
- Endpoint: `/api/CRM/Lead`
- Authentication configured using Basic Auth.
- Customer creation request was executed.
- Response was verified with Status 200 and customer details.

 Postman Features Used

- Environment variables
- Base URL variable
- Authentication variables
- GET and POST requests
- Response validation
- Postman collection export

 2. Manual Testing

Test cases and field validations were prepared for:

- Sign Up
- Forgot Password
- Sign in with OTP
- Login

The manual testing workbook contains:

- Test Cases
- Field Validations
- Bugs

 3. Automation Testing

Automation was implemented using:

- Java
- Maven
- Selenium WebDriver
- TestNG

 Automation Scenarios

- Login journey using parameterization and validation
- Punch-In toast/popup validation
- Add Customer using parameterization and validation

 Project Structure

```text
fieldforce-qa-machine-test/
├── Automation/
│   └── fieldforceconnect-automation.zip
├── FieldForce-Postman-API-Testing.postman_collection.json
├── FieldForce_Manual_Testing_.xlsx
└── README.md
