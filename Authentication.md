# Authentication

## About

Authentication is the process of verifying the identity of a user, device, or system before granting access to resources.

It answers the question:

**"Who are you?"**

Authentication is the first step in securing systems and is commonly followed by **Authorization**, which determines what an authenticated user is allowed to do.

---

# Authentication vs Authorization

| Authentication | Authorization |
|---------------|---------------|
| Verifies Identity | Determines Permissions |
| Happens First | Happens After Authentication |
| Example: Login | Example: Access Control |

---

# Authentication Factors

Authentication methods are generally based on one or more factors.

## 1. Something You Know

Examples

- Password
- PIN
- Security Questions

---

## 2. Something You Have

Examples

- Smartphone
- OTP Token
- Smart Card
- Security Key

---

## 3. Something You Are

Examples

- Fingerprint
- Face Recognition
- Iris Scan
- Voice Recognition

---

## 4. Somewhere You Are

Examples

- GPS Location
- Office Network
- Trusted Device Location

---

## 5. Something You Do

Examples

- Typing Pattern
- Mouse Movement
- Signature Dynamics

---

# Types of Authentication

## 1. Password Authentication

The user enters a username and password.

Advantages

- Easy to Implement
- Widely Used

Disadvantages

- Weak Passwords
- Password Reuse
- Phishing Risk

---

## 2. One-Time Password (OTP)

A temporary password valid for a single login session.

Types

- SMS OTP
- Email OTP
- Authenticator App OTP

Advantages

- Extra Security
- Short Validity

---

## 3. Multi-Factor Authentication (MFA)

MFA requires two or more authentication factors.

Example

```
Username + Password
        +
OTP from Mobile App
```

Advantages

- Strong Protection
- Reduces Account Takeover Risk

---

## 4. Biometric Authentication

Uses unique biological characteristics.

Examples

- Fingerprint
- Face Unlock
- Iris Scan

Advantages

- Convenient
- Difficult to Copy

---

## 5. Certificate-Based Authentication

Uses digital certificates to verify identity.

Commonly Used In

- HTTPS
- VPN
- Enterprise Networks

---

## 6. Token-Based Authentication

After successful login, the server issues a token that is used for future requests.

Examples

- JWT (JSON Web Token)
- OAuth Access Token

Common Uses

- Web Applications
- REST APIs
- Mobile Apps

---

# Single Sign-On (SSO)

SSO allows users to log in once and access multiple applications without logging in again.

Examples

- Google Account
- Microsoft Account
- Enterprise Portals

Advantages

- Better User Experience
- Fewer Passwords
- Centralized Authentication

---

# Password Security Best Practices

- Use Strong Passwords
- Avoid Password Reuse
- Enable MFA
- Use Password Managers
- Change Default Passwords
- Never Share Passwords

---

# Common Authentication Attacks

## Phishing

Attackers trick users into revealing credentials.

---

## Brute Force Attack

Repeatedly guessing passwords until the correct one is found.

---

## Credential Stuffing

Using leaked usernames and passwords from previous data breaches.

---

## Password Spraying

Trying one common password against many accounts.

---

## Keylogging

Recording keyboard input to steal credentials.

---

## Session Hijacking

Stealing an authenticated user's active session.

---

# Authentication Protocols

| Protocol | Purpose |
|----------|---------|
| Kerberos | Secure Network Authentication |
| LDAP | Directory Authentication |
| RADIUS | Remote User Authentication |
| TACACS+ | Network Device Authentication |
| OAuth 2.0 | Authorization Framework |
| OpenID Connect | User Authentication |

---

# Real-Life Example

When logging into an online banking application:

1. Enter Username and Password.
2. Receive an OTP on the registered mobile phone.
3. Enter the OTP.
4. Access is granted after successful verification.

This is an example of **Multi-Factor Authentication (MFA)**.

---

# Advantages of Strong Authentication

- Prevents Unauthorized Access
- Protects Sensitive Data
- Reduces Identity Theft
- Improves Compliance
- Increases User Trust

---

# Best Practices

- Enable MFA Wherever Possible
- Use Password Managers
- Use Long, Unique Passwords
- Lock Accounts After Multiple Failed Attempts
- Monitor Login Activity
- Keep Authentication Systems Updated

---

# Interview Questions

1. What is Authentication?
2. What is the difference between Authentication and Authorization?
3. What are the different authentication factors?
4. What is Multi-Factor Authentication (MFA)?
5. What is Biometric Authentication?
6. What is Single Sign-On (SSO)?
7. What is the purpose of OTP?
8. What is Credential Stuffing?
9. Name two authentication protocols.
10. Why is MFA more secure than password-only authentication?

---

# Summary

Topics Covered

- Authentication
- Authorization
- Authentication Factors
- Password Authentication
- OTP
- MFA
- Biometric Authentication
- Certificate-Based Authentication
- Token-Based Authentication
- SSO
- Authentication Attacks
- Authentication Protocols
- Best Practices
- Interview Questions

Authentication is a fundamental security process that verifies identity before granting access. Combining strong passwords with Multi-Factor Authentication significantly improves security against modern cyber threats.

**End of File**
