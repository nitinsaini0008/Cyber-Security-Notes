# Cross-Site Scripting (XSS)

## About

Cross-Site Scripting (XSS) is a web application vulnerability that allows attackers to inject malicious client-side scripts into web pages viewed by other users.

When the victim visits the affected webpage, the malicious script executes inside the victim's browser, potentially allowing attackers to steal session cookies, hijack accounts, modify webpage content, or perform actions on behalf of the user.

---

# What is XSS?

XSS occurs when an application accepts untrusted user input and displays it in a web page without proper validation or output encoding.

Instead of displaying the input as plain text, the browser executes it as JavaScript.

---

# How XSS Works

```
Attacker

     │
Injects Malicious Script

     │
Vulnerable Website

     │
Victim Opens Webpage

     │
Browser Executes Script

     │
Attacker Gains Information
```

---

# Types of XSS

## 1. Stored XSS (Persistent XSS)

### Definition

The malicious script is permanently stored on the web server or database.

Whenever users access the affected page, the script automatically executes.

### Examples

- Blog Comments
- Forum Posts
- User Profiles
- Product Reviews

### Risk

High because every visitor may be affected.

---

## 2. Reflected XSS

### Definition

The malicious script is reflected from the web server and immediately executed when the victim clicks a specially crafted URL.

### Examples

- Search Pages
- Login Error Messages
- Contact Forms

### Risk

Requires the victim to open a malicious link.

---

## 3. DOM-Based XSS

### Definition

The vulnerability exists in client-side JavaScript.

The server response is safe, but JavaScript modifies the webpage using untrusted input.

### Example

JavaScript reads data from the URL and inserts it directly into the page without validation.

---

# Common Causes

- No Input Validation
- No Output Encoding
- Unsafe JavaScript Functions
- Poor Secure Coding Practices
- Trusting User Input

---

# Possible Impact

- Session Cookie Theft
- Session Hijacking
- Account Takeover
- Website Defacement
- Fake Login Forms
- Credential Theft
- Malware Distribution
- Phishing Attacks

---

# Example Scenario

A website allows users to post comments.

An attacker submits a comment containing malicious JavaScript.

The application stores the comment without sanitizing it.

Every user who views the page executes the malicious script in their browser.

---

# Prevention Techniques

## 1. Input Validation

Accept only expected input.

Examples

- Allow only valid characters
- Restrict input length
- Reject malicious input

---

## 2. Output Encoding

Convert special characters into safe HTML entities before displaying user input.

This prevents browsers from interpreting the content as executable code.

---

## 3. Content Security Policy (CSP)

CSP restricts which scripts can execute within a webpage.

Benefits

- Blocks Unauthorized Scripts
- Reduces XSS Risk

---

## 4. Secure Cookies

Configure cookies using:

- HttpOnly
- Secure
- SameSite

Benefits

- Helps Protect Session Cookies
- Reduces Cookie Theft Risk

---

## 5. Safe JavaScript Practices

Avoid dangerous functions such as:

- eval()
- document.write()
- innerHTML (with untrusted input)

Prefer safer alternatives like:

- textContent
- createElement()

---

# Detection Methods

- Manual Security Testing
- Source Code Review
- Penetration Testing
- Vulnerability Scanners
- Browser Developer Tools

---

# Security Testing Tools

- Burp Suite
- OWASP ZAP
- Nikto
- Acunetix
- Nessus

---

# Best Practices

- Validate All User Input
- Encode Output
- Enable Content Security Policy
- Use Secure Cookies
- Keep Frameworks Updated
- Perform Regular Security Testing
- Avoid Inline JavaScript
- Follow Secure Coding Guidelines

---

# XSS vs SQL Injection

| Feature | XSS | SQL Injection |
|---------|-----|---------------|
| Target | User's Browser | Database |
| Executes | JavaScript | SQL Queries |
| Main Goal | Steal User Data | Access Database |
| Affects | Website Visitors | Backend Database |
| Prevention | Output Encoding, CSP | Parameterized Queries |

---

# Real-Life Example

A social media website allows users to post comments.

An attacker submits a malicious script inside a comment.

When other users view the comment, the script steals their session cookies and sends them to the attacker.

The website could have prevented this attack through input validation, output encoding, secure cookies, and a Content Security Policy.

---

# Interview Questions

1. What is Cross-Site Scripting (XSS)?
2. What are the three main types of XSS?
3. What is the difference between Stored and Reflected XSS?
4. What is DOM-Based XSS?
5. How does Content Security Policy (CSP) help prevent XSS?
6. Why is output encoding important?
7. What are HttpOnly cookies?
8. Name three tools used to detect XSS.
9. What is the difference between XSS and SQL Injection?
10. List five best practices to prevent XSS.

---

# Summary

Topics Covered

- Cross-Site Scripting (XSS)
- Stored XSS
- Reflected XSS
- DOM-Based XSS
- Causes
- Impact
- Prevention Techniques
- Content Security Policy
- Secure Cookies
- Detection Methods
- Security Tools
- XSS vs SQL Injection
- Interview Questions

Cross-Site Scripting (XSS) is one of the most common web application vulnerabilities. Proper input validation, output encoding, secure cookies, and Content Security Policy (CSP) significantly reduce the risk of XSS attacks and help protect users from malicious scripts.

**End of File**
