# Vulnerable Example

## Insecure Query Pattern

A common cause of SQL injection is building SQL queries by directly concatenating user input into the statement.

Example of insecure logic:

```sql
SELECT * FROM Users
WHERE username = '[user_input]'
AND password = '[user_input]';
