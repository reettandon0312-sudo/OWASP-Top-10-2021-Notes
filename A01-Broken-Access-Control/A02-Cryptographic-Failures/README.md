A02:2021 – Cryptographic Failures

What are Cryptographic Failures?
Cryptographic Failures occur when an application does not properly protect sensitive data using encryption. This can expose information such as passwords, credit card details, personal information, or business data to attackers.

Common Causes
•	Sensitive data is stored without encryption. 
•	Website uses HTTP instead of HTTPS. 
•	Weak or outdated encryption algorithms (such as MD5 or SHA-1). 
•	Hard-coded passwords or encryption keys. 
•	Weak password hashing. 
•	Poor key management. 
•	Weak or predictable random number generation. 

Impact
•	Password theft. 
•	Credit card information exposed. 
•	Personal data leakage. 
•	Identity theft. 
•	Financial loss. 
•	Loss of customer trust. 

How to Prevent
•	Always use HTTPS (TLS) for secure communication. 
•	Encrypt sensitive data stored in databases. 
•	Store passwords using strong hashing algorithms like bcrypt, Argon2, or PBKDF2. 
•	Avoid weak algorithms like MD5 and SHA-1. 
•	Use strong, randomly generated encryption keys. 
•	Remove sensitive data when it is no longer needed. 
•	Regularly update encryption methods and security settings. 

Example Attack Scenarios
Scenario 1 – Unencrypted Database
A website stores users' credit card details without proper encryption.
If an attacker gains database access through a vulnerability such as SQL Injection, they can read all credit card numbers.

