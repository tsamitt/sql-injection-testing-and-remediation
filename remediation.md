# Remediation

## 1. Use Parameterized Queries

Parameterized queries separate SQL logic from user-supplied values. This ensures that input is treated as data rather than executable SQL.

This is one of the most effective protections against SQL injection.

## 2. Validate Input

User input should be checked for expected type, length, and format before being processed.

Examples:

- usernames should have expected character limits
- IDs should be numeric where appropriate
- text fields should have size restrictions

## 3. Use Least Privilege

The database account used by the application should only have the minimum permissions required.

For example, a login-related function should not have permission to drop tables or perform unnecessary administrative tasks.

## 4. Store Passwords Securely

Passwords should never be stored in plaintext. Instead, they should be hashed and salted using secure password-handling methods.

## 5. Log Suspicious Activity

Unexpected input patterns, repeated login failures, and malformed requests should be logged for investigation.

## 6. Perform Security Testing

Applications should be reviewed regularly for insecure query patterns, especially around:

- login forms
- search functions
- reporting pages
- comment or request submission forms

## Conclusion

Preventing SQL injection requires secure coding habits, careful database access control, and consistent validation of user input.
