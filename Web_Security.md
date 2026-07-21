# Web Security

## About

Web Security is the practice of protecting websites, web applications, APIs, and users from cyber attacks, unauthorized access, and data breaches.

Modern web applications handle sensitive information such as passwords, banking details, personal information, and business data. Web security ensures that this information remains safe.

---

# What is Web Security?

Web Security consists of technologies, policies, and best practices used to protect web applications from vulnerabilities and attacks.

It helps protect:

- Websites
- Web Applications
- APIs
- User Accounts
- Databases
- Web Servers

---

# Objectives of Web Security

- Protect User Data
- Prevent Unauthorized Access
- Ensure Data Integrity
- Maintain Service Availability
- Secure Online Transactions

---

# Common Web Security Threats

## 1. SQL Injection (SQLi)

Attackers insert malicious SQL queries into input fields to access or manipulate databases.

Example

```
' OR '1'='1
```

Prevention

- Parameterized Queries
- Prepared Statements
- Input Validation

---

## 2. Cross-Site Scripting (XSS)

Attackers inject malicious JavaScript into web pages viewed by other users.

Types

- Stored XSS
- Reflected XSS
- DOM-Based XSS

Prevention

- Input Validation
- Output Encoding
- Content Security Policy (CSP)

---

## 3. Cross-Site Request Forgery (CSRF)

Attackers trick authenticated users into performing unwanted actions on a trusted website.

Example

A logged-in user unknowingly submits a money transfer request through a malicious webpage.

Prevention

- CSRF Tokens
- SameSite Cookies
- User Re-authentication for Sensitive Actions

---

## 4. Broken Authentication

Weak authentication mechanisms allow attackers to gain unauthorized access.

Examples

- Weak Passwords
- Session Hijacking
- Credential Stuffing

Prevention

- MFA
- Strong Password Policies
- Secure Session Management

---

## 5. Security Misconfiguration

Improper server or application settings expose systems to attacks.

Examples

- Default Passwords
- Open Directory Listing
- Unnecessary Services Enabled

Prevention

- Secure Default Configuration
- Regular Security Audits
- Timely Updates

---

## 6. File Upload Vulnerabilities

Attackers upload malicious files to execute unauthorized code.

Prevention

- Validate File Types
- Limit File Size
- Store Uploads Outside the Web Root
- Scan Uploaded Files

---

## 7. Clickjacking

Attackers trick users into clicking hidden elements on a webpage.

Prevention

- X-Frame-Options Header
- Content Security Policy (CSP)

---

## HTTPS

HTTPS secures communication between browsers and web servers using TLS encryption.

Benefits

- Encrypts Data
- Protects User Privacy
- Prevents Data Tampering
- Verifies Website Identity

---

# Secure Authentication

Best Practices

- Use MFA
- Strong Password Policy
- Password Hashing
- Secure Session Cookies
- Automatic Session Timeout

---

# Secure Coding Practices

- Validate User Input
- Sanitize Output
- Use Prepared Statements
- Handle Errors Securely
- Avoid Hardcoded Credentials
- Keep Dependencies Updated

---

# HTTP Security Headers

Common Headers

| Header | Purpose |
|---------|---------|
| Content-Security-Policy | Prevent XSS |
| X-Frame-Options | Prevent Clickjacking |
| X-Content-Type-Options | Prevent MIME Sniffing |
| Strict-Transport-Security (HSTS) | Force HTTPS |
| Referrer-Policy | Control Referrer Information |

---

# Web Application Firewall (WAF)

A WAF filters HTTP/HTTPS traffic and blocks malicious requests before they reach the web application.

Benefits

- Blocks SQL Injection
- Blocks XSS
- Protects APIs
- Monitors Traffic

Examples

- Cloudflare WAF
- AWS WAF
- Azure WAF

---

# Secure Cookies

Cookies should use:

- HttpOnly
- Secure
- SameSite

These attributes help protect session cookies from theft and misuse.

---

# Best Practices

- Enable HTTPS Everywhere
- Keep Software Updated
- Perform Regular Security Testing
- Use Web Application Firewalls
- Enable Logging and Monitoring
- Perform Regular Backups
- Follow the Principle of Least Privilege
- Review Application Permissions

---

# Real-Life Example

An online shopping website validates user input, uses HTTPS, stores passwords securely with hashing, enables MFA for administrators, and deploys a WAF.

These controls help protect customer accounts and payment information from common web attacks.

---

# Interview Questions

1. What is Web Security?
2. Why is HTTPS important?
3. What is SQL Injection?
4. What is Cross-Site Scripting (XSS)?
5. What is CSRF?
6. What is a Web Application Firewall (WAF)?
7. What are HTTP Security Headers?
8. Why should passwords be hashed?
9. What are secure cookies?
10. List five Web Security best practices.

---

# Summary

Topics Covered

- Web Security
- SQL Injection
- XSS
- CSRF
- Broken Authentication
- Security Misconfiguration
- File Upload Vulnerabilities
- Clickjacking
- HTTPS
- Secure Coding
- HTTP Security Headers
- Web Application Firewall
- Secure Cookies
- Best Practices
- Interview Questions

Web Security is essential for protecting modern websites and web applications. Combining secure coding practices, HTTPS, strong authentication, and continuous monitoring helps reduce the risk of cyber attacks and data breaches.

**End of File**
