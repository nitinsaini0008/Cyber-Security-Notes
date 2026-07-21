# OWASP Top 10

## About

The **OWASP Top 10** is a globally recognized awareness document published by the **Open Worldwide Application Security Project (OWASP)**. It lists the most critical security risks affecting web applications and helps developers, testers, and security professionals build more secure software.

---

# What is OWASP?

OWASP (Open Worldwide Application Security Project) is a non-profit organization dedicated to improving software security through free resources, tools, documentation, and community projects.

---

# Why is the OWASP Top 10 Important?

- Identifies common web application vulnerabilities
- Helps developers build secure applications
- Improves security awareness
- Reduces the risk of cyber attacks
- Used in security audits and penetration testing

---

# OWASP Top 10 (2021)

## A01:2021 – Broken Access Control

### Description

Broken Access Control occurs when users can access resources or perform actions beyond their intended permissions.

### Examples

- Accessing another user's account
- Viewing confidential files
- Bypassing authorization checks

### Prevention

- Implement Role-Based Access Control (RBAC)
- Validate permissions on the server
- Deny access by default
- Perform regular access control testing

---

## A02:2021 – Cryptographic Failures

### Description

Sensitive information is exposed because encryption is missing, weak, or implemented incorrectly.

### Examples

- Storing passwords in plain text
- Using weak encryption algorithms
- Sending sensitive data over HTTP

### Prevention

- Use HTTPS
- Use AES-256 for encryption
- Store passwords using secure hashing algorithms
- Protect encryption keys

---

## A03:2021 – Injection

### Description

Injection vulnerabilities occur when untrusted input is interpreted as commands or queries.

### Examples

- SQL Injection
- NoSQL Injection
- Command Injection

### Prevention

- Parameterized Queries
- Prepared Statements
- Input Validation
- Least Privilege

---

## A04:2021 – Insecure Design

### Description

Security weaknesses introduced during application design rather than coding.

### Examples

- Missing rate limiting
- Weak authentication workflows
- Insecure business logic

### Prevention

- Secure Design Principles
- Threat Modeling
- Security Reviews
- Secure SDLC

---

## A05:2021 – Security Misconfiguration

### Description

Incorrect or insecure system configurations expose applications to attacks.

### Examples

- Default passwords
- Unnecessary services
- Directory listing enabled

### Prevention

- Secure default configurations
- Remove unused services
- Regular configuration reviews
- Apply security patches

---

## A06:2021 – Vulnerable and Outdated Components

### Description

Applications use libraries or software containing known security vulnerabilities.

### Examples

- Outdated frameworks
- Unsupported software
- Unpatched operating systems

### Prevention

- Keep software updated
- Remove unused libraries
- Monitor security advisories
- Perform vulnerability scans

---

## A07:2021 – Identification and Authentication Failures

### Description

Weak authentication allows attackers to compromise user accounts.

### Examples

- Weak passwords
- Session hijacking
- Credential stuffing

### Prevention

- Enable MFA
- Strong password policies
- Secure session management
- Account lockout policies

---

## A08:2021 – Software and Data Integrity Failures

### Description

Applications fail to verify the integrity of software updates, plugins, or data.

### Examples

- Installing unsigned software
- Insecure CI/CD pipelines
- Untrusted updates

### Prevention

- Verify digital signatures
- Protect CI/CD pipelines
- Validate software integrity

---

## A09:2021 – Security Logging and Monitoring Failures

### Description

Poor logging and monitoring delay the detection and response to attacks.

### Examples

- Missing audit logs
- No alert generation
- Incomplete incident records

### Prevention

- Enable centralized logging
- Monitor security events
- Generate real-time alerts
- Regularly review logs

---

## A10:2021 – Server-Side Request Forgery (SSRF)

### Description

An attacker tricks a server into making requests to unintended internal or external resources.

### Examples

- Accessing internal APIs
- Retrieving cloud metadata
- Internal network scanning

### Prevention

- Validate URLs
- Restrict outbound requests
- Use allowlists
- Segment internal networks

---

# OWASP Top 10 Summary

| Rank | Vulnerability |
|------|---------------|
| A01 | Broken Access Control |
| A02 | Cryptographic Failures |
| A03 | Injection |
| A04 | Insecure Design |
| A05 | Security Misconfiguration |
| A06 | Vulnerable and Outdated Components |
| A07 | Identification and Authentication Failures |
| A08 | Software and Data Integrity Failures |
| A09 | Security Logging and Monitoring Failures |
| A10 | Server-Side Request Forgery (SSRF) |

---

# Best Practices

- Validate all user input
- Use HTTPS everywhere
- Implement MFA
- Follow the Principle of Least Privilege
- Keep software updated
- Use secure coding practices
- Perform regular penetration testing
- Enable logging and monitoring
- Conduct security code reviews
- Follow the Secure Software Development Life Cycle (SSDLC)

---

# Real-Life Example

An e-commerce website uses parameterized SQL queries, HTTPS, MFA for administrators, role-based access control, centralized logging, and regularly updates third-party libraries.

These security controls significantly reduce the risk of vulnerabilities listed in the OWASP Top 10.

---

# Interview Questions

1. What is OWASP?
2. What is the OWASP Top 10?
3. What is Broken Access Control?
4. What is an Injection attack?
5. What are Cryptographic Failures?
6. Why are software updates important for security?
7. What is SSRF?
8. Why is logging important in cyber security?
9. What is Security Misconfiguration?
10. How can organizations reduce OWASP Top 10 risks?

---

# Summary

Topics Covered

- OWASP
- OWASP Top 10 (2021)
- Web Application Vulnerabilities
- Secure Design
- Secure Coding
- Logging & Monitoring
- Best Practices
- Interview Questions

The OWASP Top 10 serves as a practical guide for identifying and mitigating the most critical web application security risks. Understanding these vulnerabilities is essential for developers, penetration testers, security analysts, and anyone involved in application security.

**End of File**
