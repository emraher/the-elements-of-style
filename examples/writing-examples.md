# Writing Examples Test Suite

This file contains examples to verify the Elements of Style skill works correctly and to demonstrate improvements.

## Test 1: Active Voice (Rule 10)

### Bad Examples

```
The database was queried by the application.
The error was logged by the system.
The user's request will be processed by the server.
Improvements have been made to the codebase.
```

### Good Examples

```
The application queries the database.
The system logs the error.
The server processes the user's request.
We improved the codebase.
```

## Test 2: Positive Form (Rule 11)

### Bad Examples

```
The test did not pass.
The function does not return a value when the input is invalid.
He was not very often on time.
The configuration is not correct.
```

### Good Examples

```
The test failed.
The function returns null for invalid input.
He usually came late.
The configuration is incorrect.
```

## Test 3: Concrete Language (Rule 12)

### Bad Examples

```
There was a problem with the system.
The application experienced issues during deployment.
Performance improvements were observed.
The user interface underwent modifications.
```

### Good Examples

```
The system crashed at 3:14 PM.
The application failed to start: missing environment variable DATABASE_URL.
API response time decreased from 450ms to 180ms.
We redesigned the navigation menu and moved the search bar to the header.
```

## Test 4: Omit Needless Words (Rule 13)

### Bad Examples

```
The question as to whether we should proceed is still being considered.
In spite of the fact that the tests passed, there are still concerns.
This is a feature that will be useful for many users.
He is a developer who has experience with React.
In order to improve performance, we cached the results.
```

### Good Examples

```
Whether we should proceed is still being considered.
Though the tests passed, concerns remain.
This feature will benefit many users.
He has React experience.
To improve performance, we cached the results.
```

## Test 5: Keep Related Words Together (Rule 16)

### Bad Examples

```
The function only works when authenticated.
He found almost all the bugs in the codebase.
The user can, by clicking the button, submit the form.
```

### Good Examples

```
The function works only when authenticated.
He found almost all bugs in the codebase.
The user can submit the form by clicking the button.
```

## Test 6: Git Commit Messages

### Bad Examples

```
Fixed bugs
Updated files
Changes were made to improve the API
The authentication system was refactored
```

### Good Examples

```
Fix validation error in user registration
Update dependencies to patch security vulnerabilities
Improve API: Add rate limiting and response caching
Refactor authentication to use JWT tokens
```

## Test 7: Error Messages

### Bad Examples

```
An error occurred.
The operation could not be completed.
Invalid input was provided.
The file was not able to be opened.
```

### Good Examples

```
Error: Database connection timeout after 30s.
Operation failed: Insufficient permissions to write to /var/log.
Invalid email format: must include @ symbol.
Cannot open file: /config/app.yml not found.
```

## Test 8: API Documentation

### Bad Examples

```
This endpoint can be used to retrieve user information.
The data will be returned in JSON format.
Errors should be handled by the client application.
The response will be cached by the server.
```

### Good Examples

```
This endpoint retrieves user information.
Returns JSON data.
Clients must handle errors.
The server caches responses for 5 minutes.
```

## Test 9: Code Comments

### Bad Examples

```
// This function is used for the purpose of validating the user's input
// In the event that the validation fails, an error will be thrown
// This is a helper function that handles the case where the user is not authenticated
```

### Good Examples

```
// Validates user input
// Throws error if validation fails
// Returns 401 for unauthenticated users
```

## Test 10: Multiple Rules Combined

### Bad Example

```
The new feature that was added to the system is not yet available
to all users due to the fact that there are still some issues that
need to be resolved. It is expected that the feature will be rolled
out in the near future once the problems have been fixed.
```

### Good Example

```
We added a new feature but haven't released it to all users yet.
Three bugs block the rollout. We expect to fix them and release
the feature next week.
```

**Improvements applied:**

- Rule 10: Active voice ("We added" not "was added")
- Rule 11: Positive form ("Three bugs block" not "issues need to be resolved")
- Rule 12: Concrete ("next week" not "near future")
- Rule 13: Omit needless ("due to the fact that" → removed)

## Expected Skill Behavior

When given bad examples, the skill should:

1. Identify which rule(s) are violated
2. Explain why the original is weak
3. Provide a corrected version
4. Reference specific rule numbers (e.g., "Rule 10: Use active voice")

When given good examples, the skill should:

1. Confirm they follow the principles
2. Identify which rules they exemplify
3. Optionally suggest minor refinements if applicable
