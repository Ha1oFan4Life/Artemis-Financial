Artemis Financial – Software Security Project Reflection

Who was the client and what issue did the company want you to address?
The client was Artemis Financial, a financial services company that needed to improve the security of their communications and application infrastructure. They wanted me to address issues related to data integrity and secure communication, specifically by implementing encryption, securing client-server connections, and ensuring the codebase was free of known vulnerabilities.

What did you do well when finding software security vulnerabilities? Why is secure coding important?
I did a thorough job identifying potential weak points, like the lack of encrypted data transmission and the absence of a checksum for verifying data integrity. I implemented SHA-256 hashing and HTTPS to address these issues. Secure coding is critical because it prevents attackers from exploiting vulnerabilities that could lead to data breaches, financial losses, or damage to the company's reputation. Secure software strengthens customer trust and ensures regulatory compliance.

Which part of the vulnerability assessment was challenging or helpful?
One of the most challenging parts was setting up the OWASP Dependency-Check tool with an NVD API key, but it was also very helpful because it systematically confirmed that no known vulnerabilities were present in the final code. It gave me confidence that the changes I made truly improved the system’s security.

How did you increase layers of security? What would you use for future assessments?
I increased security layers by:

    Adding SHA-256 hashing to verify data integrity.

    Enabling HTTPS using a properly configured self-signed certificate.

    Running a static code analysis using OWASP Dependency-Check to verify dependencies.

In the future, I would also incorporate tools like SonarQube for deeper code quality checks and possibly use a dynamic analysis tool like OWASP ZAP to scan running applications for security weaknesses.

How did you make sure the code and software application were functional and secure? How did you check for new vulnerabilities after refactoring?
I manually tested the /hash endpoint to verify that the application functioned correctly under HTTPS. After refactoring, I ran a static code analysis with OWASP Dependency-Check to ensure that no new vulnerabilities were introduced through the code or any project dependencies.

What resources, tools, or coding practices will help in the future?

    SHA-256 for hashing and ensuring data integrity.

    Java Keytool for generating certificates.

    OWASP Dependency-Check for static analysis.

    Following secure coding practices such as modularizing the code and using strong encryption. These tools and practices will definitely be useful in any future security-related development tasks.

What might you show future employers from this assignment?
I would show employers the full secure software solution I developed:

    The refactored, functional Spring Boot application with HTTPS and SHA-256 checksum validation.

    Documentation of the security practices I followed.

    Evidence from the OWASP Dependency-Check scan showing 0 vulnerabilities. This project demonstrates my ability to recognize vulnerabilities, refactor code securely, implement encryption, and validate my work with industry-standard tools.
