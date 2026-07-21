# SQL Injection (SQLi)

## About

SQL Injection (SQLi) is one of the most common and dangerous web application vulnerabilities. It occurs when an attacker injects malicious SQL commands into user input, causing the application to execute unintended database queries.

A successful SQL Injection attack can lead to unauthorized access, data theft, modification of records, or even complete control of the database.

---

# What is SQL Injection?

SQL Injection is a code injection attack where malicious SQL statements are inserted into application inputs that interact with a database.

Instead of treating user input as data, the application mistakenly treats it as part of an SQL query.

---

# How SQL Injection Works

Normal Login

```
User Input

Username: admin
Password: admin123

↓

Application

↓

Database Query

↓

Access Granted
```

---

Vulnerable Login

```
Username:

' OR '1'='1

↓

Database Query Changes

↓

Authentication Bypassed
```

---

# Causes of SQL Injection

- No Input Validation
- Dynamic SQL Queries
- Poor Error Handling
- Lack of Parameterized Queries
- Insecure Coding Practices

---

# Types of SQL Injection

## 1. In-Band SQL Injection

The attacker receives results using the same communication channel.

Types

- Error-Based SQL Injection
- Union-Based SQL Injection

---

## 2. Blind SQL Injection

The application does not display database errors, but attackers infer information through responses.

Types

- Boolean-Based Blind SQL Injection
- Time-Based Blind SQL Injection

---

## 3. Out-of-Band SQL Injection

Data is retrieved using a different communication channel.

Example

- DNS Requests
- HTTP Requests

---

# Example of a Vulnerable Query

```sql
SELECT * FROM users
WHERE username = 'admin'
AND password = 'password';
```

If user input is directly inserted into the query without validation, the application becomes vulnerable.

---

# Possible Impact

- Authentication Bypass
- Data Theft
- Data Modification
- Data Deletion
- Privilege Escalation
- Database Takeover
- Remote Code Execution (in some cases)

---

# Databases Commonly Targeted

- MySQL
- Microsoft SQL Server
- PostgreSQL
- Oracle Database
- SQLite
- MariaDB

---

# Prevention Techniques

## 1. Parameterized Queries

Separate SQL commands from user input.

Benefits

- Prevents SQL Injection
- Recommended Best Practice

---

## 2. Prepared Statements

Prepared statements ensure that user input is treated as data rather than executable SQL.

---

## 3. Input Validation

Validate all user input.

Examples

- Length Checks
- Allowed Characters
- Data Type Validation

---

## 4. Least Privilege

Database accounts should only have the permissions they require.

Example

- Read Only
- Limited Insert Access

Avoid using administrator accounts for applications.

---

## 5. Stored Procedures

Stored procedures can improve security when implemented correctly.

---

## 6. Web Application Firewall (WAF)

A WAF can detect and block many SQL Injection attempts before they reach the application.

---

# Secure Coding Best Practices

- Never Trust User Input
- Validate Server-Side Input
- Escape Special Characters When Necessary
- Use ORM Frameworks Carefully
- Keep Database Software Updated
- Log Suspicious Activity
- Perform Security Testing

---

# SQL Injection Detection

Common methods include:

- Manual Security Testing
- Vulnerability Scanners
- Penetration Testing
- Source Code Review
- Web Application Firewalls
- Security Audits

---

# Popular Security Tools

- Burp Suite
- OWASP ZAP
- SQLMap
- Nessus
- Acunetix

---

# Real-Life Example

An online shopping website uses a login form connected to a database.

The developers concatenate user input directly into SQL queries without validation.

An attacker submits specially crafted input that changes the query logic and gains unauthorized access to customer accounts.

The vulnerability could have been prevented by using parameterized queries, prepared statements, and proper input validation.

---

# Best Practices

- Use Parameterized Queries
- Use Prepared Statements
- Validate Every Input
- Apply Least Privilege
- Enable Logging
- Keep Software Updated
- Perform Regular Penetration Testing
- Use HTTPS
- Deploy a Web Application Firewall

---

# Interview Questions

1. What is SQL Injection?
2. Why is SQL Injection dangerous?
3. Name the different types of SQL Injection.
4. What is Blind SQL Injection?
5. What are Parameterized Queries?
6. What are Prepared Statements?
7. How does a Web Application Firewall help prevent SQL Injection?
8. What is the Principle of Least Privilege?
9. Name three tools used to detect SQL Injection vulnerabilities.
10. List five best practices to prevent SQL Injection.

---

# Summary

Topics Covered

- SQL Injection
- Types of SQL Injection
- Causes
- Database Targets
- Prevention Techniques
- Secure Coding
- Detection Methods
- Security Tools
- Best Practices
- Interview Questions

SQL Injection remains one of the most serious web application vulnerabilities. By using parameterized queries, validating input, applying least privilege, and following secure coding practices, developers can greatly reduce the risk of SQL Injection attacks.

**End of File**
