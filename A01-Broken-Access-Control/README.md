A01:2021 – Broken Access Control

What is Broken Access Control?
Broken Access Control happens when a website or application does not properly check what a user is allowed to do. Because of this, an attacker can access, modify, or delete data that belongs to other users or even gain admin privileges.
Simple Example:
•	User A logs into their account. 
•	They change the URL from:
https://example.com/account?id=101
to
https://example.com/account?id=102
•	If the application shows User B's account without checking permissions, it is Broken Access Control. 

Common Causes
•	Missing authorization checks. 
•	Users can access admin pages without permission. 
•	Users can edit or view other users' data. 
•	Insecure Direct Object Reference (IDOR). 
•	Poor API access control. 
•	Misconfigured CORS. 
•	JWT or session manipulation. 

Impact
•	Unauthorized access to sensitive data. 
•	Data modification or deletion. 
•	Privilege escalation (normal user becomes admin). 
•	Financial and reputational loss. 
•	Data breaches. 

How to Prevent
•	Apply the Principle of Least Privilege (users get only the permissions they need). 
•	Verify permissions on the server side. 
•	Deny access by default. 
•	Validate every request before providing data. 
•	Disable unnecessary directory listing. 
•	Log unauthorized access attempts. 
•	Use secure session management and short-lived JWT tokens. 
•	Perform regular security testing. 

Example Attack Scenario
Normal User
https://example.com/account?id=101
Attacker Changes URL
https://example.com/account?id=102
If the application displays another user's account, it is vulnerable to Broken Access Control (IDOR).
