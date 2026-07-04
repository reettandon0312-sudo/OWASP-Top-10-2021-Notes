A04:2021 – Insecure Design

What is Insecure Design?
Insecure Design means security was not considered while designing the application. Even if the code is written correctly, the application can still be vulnerable because important security controls were never included in the design.
Common Causes
•	No security planning during development. 
•	No threat modeling. 
•	Weak authentication or password recovery process. 
•	Missing business logic validation. 
•	No rate limiting. 
•	No protection against bots or automated attacks. 
•	Poor access control design. 

Impact
•	Unauthorized access. 
•	Financial loss. 
•	Business logic abuse. 
•	Automated attacks (bots). 
•	Data theft. 
•	Damage to company reputation. 

How to Prevent
•	Follow a Secure Development Lifecycle (SDLC). 
•	Perform Threat Modeling before development. 
•	Design authentication and authorization securely. 
•	Add rate limiting to prevent abuse. 
•	Validate all business logic. 
•	Write security-focused unit and integration tests. 
•	Separate application layers (frontend, backend, database). 
•	Review the design regularly for security weaknesses. 

Example Attack Scenarios
Scenario 1 – Weak Password Recovery
A website allows users to reset their password by answering simple security questions like:
•	What is your pet's name? 
•	What is your mother's maiden name? 
An attacker finds these answers on social media and resets the victim's password.
