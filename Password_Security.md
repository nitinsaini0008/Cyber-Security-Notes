# Password Security

## About

Password Security refers to the practices and techniques used to create, store, manage, and protect passwords from unauthorized access. Strong password security is one of the most effective ways to prevent cyber attacks.

---

# What is a Password?

A password is a secret combination of characters used to verify the identity of a user and protect access to systems, applications, and data.

Example

```
Username: nitin123
Password: MySecure@2026
```

---

# Characteristics of a Strong Password

A strong password should:

- Be at least 12–16 characters long
- Include uppercase letters
- Include lowercase letters
- Include numbers
- Include special characters
- Be unique for every account

Example of a Strong Password

```
N!tin@2026#Secure
```

Example of a Weak Password

```
123456
password
admin
qwerty
nitin123
```

---

# Password Attacks

## 1. Brute Force Attack

The attacker tries every possible password combination until the correct one is found.

### Prevention

- Strong Passwords
- MFA
- Account Lockout

---

## 2. Dictionary Attack

The attacker uses a predefined list of common passwords.

Example

- password
- admin
- welcome123

### Prevention

- Use Random Passwords
- Avoid Common Words

---

## 3. Credential Stuffing

Attackers use usernames and passwords leaked from previous data breaches to access other accounts.

### Prevention

- Use Different Passwords for Every Account
- Enable MFA

---

## 4. Password Spraying

Attackers try one common password against many user accounts.

Example

```
Spring2026!
```

### Prevention

- Strong Password Policy
- Account Monitoring

---

## 5. Keylogging

Malware secretly records everything typed on the keyboard.

### Prevention

- Antivirus
- MFA
- Avoid Untrusted Software

---

## Password Storage

Passwords should **never** be stored in plain text.

Instead, they should be:

- Hashed
- Salted
- Stored Securely

Example

```
Password

↓

Salt

↓

SHA-256 Hash

↓

Database
```

---

# Hashing vs Encryption

| Hashing | Encryption |
|----------|------------|
| One-Way Process | Two-Way Process |
| Cannot Be Reversed | Can Be Decrypted |
| Used for Password Storage | Used for Data Protection |

---

# Password Policies

A good password policy should require:

- Minimum 12 Characters
- Uppercase Letters
- Lowercase Letters
- Numbers
- Special Characters
- Password Expiration (where appropriate)
- Password History
- Account Lockout After Multiple Failed Attempts

---

# Multi-Factor Authentication (MFA)

MFA requires users to verify their identity using two or more authentication factors.

Example

```
Password

+

OTP

+

Fingerprint
```

Benefits

- Extra Security
- Protects Against Stolen Passwords
- Reduces Unauthorized Access

---

# Password Managers

Password managers securely generate and store strong passwords.

Popular Password Managers

- Bitwarden
- 1Password
- KeePass
- Dashlane
- LastPass

Advantages

- Strong Password Generation
- Secure Storage
- Auto Fill
- Easy Management

---

# Password Best Practices

- Use Long Passwords
- Use Unique Passwords
- Enable MFA
- Never Share Passwords
- Change Default Passwords
- Store Passwords in a Password Manager
- Avoid Writing Passwords on Paper
- Avoid Reusing Passwords
- Monitor Accounts for Suspicious Activity

---

# Common Password Mistakes

- Using Personal Information
- Reusing Passwords
- Using Short Passwords
- Sharing Passwords
- Saving Passwords in Plain Text Files
- Using Common Words

---

# Real-Life Example

A user uses the same password for email, social media, and online banking.

The password is leaked during a data breach.

An attacker uses **Credential Stuffing** to log in to the user's other accounts successfully.

This could have been prevented by:

- Using Unique Passwords
- Enabling MFA
- Using a Password Manager

---

# Interview Questions

1. What is Password Security?
2. What makes a password strong?
3. What is the difference between Hashing and Encryption?
4. What is Credential Stuffing?
5. What is Password Spraying?
6. Why should passwords be hashed?
7. What is MFA?
8. What is a Password Manager?
9. Why should passwords never be reused?
10. List five password security best practices.

---

# Summary

Topics Covered

- Password Security
- Strong Passwords
- Password Attacks
- Password Storage
- Hashing
- Encryption
- Password Policies
- MFA
- Password Managers
- Best Practices
- Interview Questions

Strong password security combined with Multi-Factor Authentication and secure password storage significantly reduces the risk of unauthorized access and protects sensitive information from cyber threats.

**End of File**
