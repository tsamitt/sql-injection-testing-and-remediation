# Attack Explanation

## What Is SQL Injection

SQL injection is a vulnerability that happens when an application allows untrusted input to alter a database query.

Instead of treating input only as data, the application accidentally allows it to change the logic of the SQL statement.

## Security Risk

If a login form, search field, or request form is not safely designed, an attacker may try to manipulate the query to:

- bypass authentication
- read data they should not access
- change stored records
- remove database content
- interfere with application behavior

## Example Scenario

Imagine a login page that sends a username and password into a SQL query without parameterization.

If the application directly inserts user input into the SQL statement, the attacker may be able to cause the database to return results it should not return.

## Why It Matters

SQL injection is dangerous because a single vulnerable input field can expose an entire application database if controls are weak.

Applications that store user accounts, service requests, comments, or attachments are all potential targets if database interaction is not secured properly.
