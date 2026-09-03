 FieldForceConnect QA Machine Test

 Overview
This repository contains my QA Machine Test work for FieldForceConnect.

 1. Postman API Testing

 Environment
- Environment: FieldForce Test
- Base URL: https://test.fieldforceconnect.com

 API Tests Performed

Login - Valid Credentials
- Method: POST
- Endpoint: `/api/account/authenticate`
- Valid credentials were used through Postman environment variables.
- Response verified successfully.

 Login - Invalid Credentials
- Method: POST
- Endpoint: `/api/account/authenticate`
- Invalid password was used.
- Response verified with an authentication error message.

 Add Customer
- Method: POST
- Endpoint: `/api/CRM/Lead`
- Authentication configured using Basic Auth.
- Customer creation request was executed successfully.
- Response verified with Status 200 and customer details.

 Postman Features Used
- Environment variables
- Base URL variable
- Authentication variables
- GET request
- POST request
- Response validation
- Postman collection export

2. Manual Testing

Test cases and field validations for:
- Sign Up
- Forgot Password
- Sign in with OTP
- Login

 3. Automation Testing

Planned/implemented using:
- Java
- Maven
- Selenium
- TestNG/Cucumber

 Automation Scenarios
- Login journey using parametrization
- Punch-In toast/popup validation
- Add Customer using parametrization
