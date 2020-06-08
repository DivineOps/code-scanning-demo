# code-scanning-demo

This demo code will trigger 3 alerts from code-scanning with CodeQL, and 2 alerts from secret scanning:

### Code scanning
Incorrect suffix check. This suffix check is missing a length comparison to correctly handle lastIndexOf returning -1.

### Code scanning - SQL Injection
Database query built from user-controlled sources. This query depends on a user-provided value.

### Code scanning
Missing rate limiting. This route handler performs a database access, but is not rate-limited.

