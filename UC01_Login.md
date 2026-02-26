# UC01 - Login

## Use Case Description
Allows registered users (Students, Teachers, and Admins) to authenticate and access the LearnFlix system.

## Actors
- Student
- Teacher
- Admin

## Pre-conditions
- User must have a valid account in the system
- System must be operational
- User must have internet connectivity

## Post-conditions
- User is authenticated and granted access to appropriate dashboard
- Session is established for the user

## Main Flow
1. User navigates to the login page
2. User enters username/email and password
3. System validates the credentials
4. System authenticates the user
5. System redirects user to the appropriate dashboard based on role
6. Session is established

## Alternative Flows
- **Invalid credentials**: System displays error message and prompts user to re-enter credentials
- **Account locked/disabled**: System displays appropriate message
- **Forgot password**: User can initiate password reset process

## Exception Flows
- System failure during authentication: Error message displayed
- Network connectivity issues: Appropriate error handling

## Business Rules
- Password must meet security requirements
- Account lockout after multiple failed attempts
- Session timeout after period of inactivity