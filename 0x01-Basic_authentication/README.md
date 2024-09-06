## 0x01. Basic Authentication

## Project Overview
This project focuses on implementing Basic Authentication for a simple API using Flask. The goal is to understand the authentication process by creating a Basic Authentication system from scratch, rather than using a pre-existing module or framework.

## Background Context
Authentication is crucial in securing web applications. This project introduces Basic Authentication, a straightforward method to protect your API endpoints. By manually implementing this system, you'll gain insight into the underlying mechanisms of authentication.

## Tasks
## 0. Simple Basic API
Objective: Set up a simple API with one model: User. Implement file-based storage for user data.

## 1. Error Handler: Unauthorized
Objective: Add a custom error handler for HTTP status code 401 with a JSON response: {"error": "Unauthorized"}. Create an endpoint to test this error handler.

## 2. Error Handler: Forbidden
Objective: Implement a custom error handler for HTTP status code 403 with a JSON response: {"error": "Forbidden"}. Create an endpoint to test this error handler.

## 3. Auth Class
Objective: Create a base class Auth for managing API authentication with methods for authentication checks and header extraction.

## 4. Define Which Routes Don't Need Authentication
Objective: Update the require_auth method in the Auth class to specify which routes should not require authentication.

## 5. Request Validation
Objective: Validate requests to secure the API. Implement methods to check authorization headers and current user validation.

## 6. Basic Auth
Objective: Create a BasicAuth class inheriting from Auth. Update the API to use this class for Basic Authentication based on environment variable AUTH_TYPE.

## 7. Basic - Base64 Part
Objective: Add a method to extract the Base64 part of the Authorization header for Basic Authentication.

## 8. Basic - Base64 Decode
Objective: Implement a method to decode Base64 strings to retrieve the original credentials.

## 9. Basic - User Credentials
Objective: Extract user credentials (email and password) from the decoded Base64 string.

## 10. Basic - User Object
Objective: Implement a method to retrieve the User instance based on email and password.

## 11. Basic - Overload current_user
Objective: Finalize Basic Authentication by overloading the current_user method to use the implemented Basic Auth methods for retrieving user instances.
