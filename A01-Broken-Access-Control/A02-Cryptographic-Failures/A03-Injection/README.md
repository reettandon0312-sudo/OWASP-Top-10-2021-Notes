A03:2021 – Injection

What is Injection?
Injection occurs when an application accepts untrusted user input and treats it as a command or query. An attacker can inject malicious code to access, modify, or delete data.
Common Types of Injection
•	SQL Injection (SQLi) – Attacks a database using malicious SQL queries. 
•	NoSQL Injection – Targets NoSQL databases like MongoDB. 
•	Command Injection – Executes operating system commands on the server. 
•	Cross-Site Scripting (XSS) – Injects malicious JavaScript into web pages. 
•	LDAP Injection – Manipulates LDAP directory queries. 
•	ORM Injection – Exploits Object Relational Mapping queries. 

Common Causes
•	User input is not validated or sanitized. 
•	Dynamic SQL queries are created by concatenating user input. 
•	No parameterized queries (prepared statements). 
•	Input is directly used in database queries or system commands. 
•	Weak input validation. 

Impact
•	Unauthorized access to sensitive data. 
•	Database modification or deletion. 
•	Authentication bypass. 
•	Remote command execution. 
•	Complete system compromise. 

How to Prevent
•	Use parameterized queries (Prepared Statements). 
•	Validate and sanitize all user input. 
•	Use server-side input validation. 
•	Avoid building SQL queries by concatenating strings. 
•	Use ORM frameworks safely. 
•	Escape special characters when dynamic queries are unavoidable. 
•	Perform regular security testing (SAST, DAST, IAST). 

Example Attack Scenarios
Scenario 1 – SQL Injection
Normal query:
SELECT * FROM users WHERE id='1';
Attacker enters:
' OR '1'='1
The query becomes:
SELECT * FROM users WHERE id='' OR '1'='1';
Since '1'='1' is always true, the database may return all user records.
