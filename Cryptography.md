# Cryptography

## About

Cryptography is the science of protecting information by converting readable data (plaintext) into an unreadable format (ciphertext). It ensures that only authorized users can access the original information.

Cryptography is widely used in banking, e-commerce, messaging applications, cloud computing, and secure communication.

---

# What is Cryptography?

Cryptography is a security technique that protects data from unauthorized access using mathematical algorithms and cryptographic keys.

It provides:

- Confidentiality
- Integrity
- Authentication
- Non-Repudiation

---

# Basic Terminology

## Plaintext

The original readable message.

Example

```
Hello World
```

---

## Ciphertext

The encrypted unreadable message.

Example

```
X7#@91P$L
```

---

## Encryption

Encryption is the process of converting plaintext into ciphertext using an encryption algorithm and a key.

```
Plaintext
     ↓
Encryption + Key
     ↓
Ciphertext
```

---

## Decryption

Decryption converts ciphertext back into plaintext using the correct key.

```
Ciphertext
      ↓
Decryption + Key
      ↓
Plaintext
```

---

# Goals of Cryptography

## 1. Confidentiality

Ensures only authorized users can read the data.

Example

- WhatsApp Messages
- Online Banking

---

## 2. Integrity

Ensures data has not been modified during transmission.

Example

- Software Downloads
- Digital Documents

---

## 3. Authentication

Verifies the identity of users or systems.

Example

- Login Systems
- Digital Certificates

---

## 4. Non-Repudiation

Prevents a sender from denying that they sent a message.

Example

- Digital Signatures
- Online Contracts

---

# Types of Cryptography

## 1. Symmetric Key Cryptography

### Definition

The same secret key is used for both encryption and decryption.

```
Sender
   ↓
Encryption
   ↓
Shared Secret Key
   ↓
Ciphertext
   ↓
Receiver
   ↓
Same Secret Key
   ↓
Decryption
```

### Advantages

- Fast
- Efficient
- Suitable for Large Data

### Disadvantages

- Key Distribution is Difficult
- Less Secure if the Key is Compromised

### Examples

- AES
- DES
- 3DES
- Blowfish

---

## 2. Asymmetric Key Cryptography

### Definition

Uses two keys:

- Public Key
- Private Key

```
Public Key
     ↓
Encryption
     ↓
Ciphertext
     ↓
Private Key
     ↓
Decryption
```

### Advantages

- Secure Key Exchange
- Supports Digital Signatures

### Disadvantages

- Slower than Symmetric Encryption

### Examples

- RSA
- ECC
- Diffie-Hellman (Key Exchange)

---

# Hashing

## Definition

Hashing converts data into a fixed-length value called a hash.

Hashing is a one-way process and cannot be reversed.

Example Algorithms

- MD5 (Not Recommended)
- SHA-1 (Deprecated)
- SHA-256
- SHA-512

Example

```
Password

↓

SHA-256

↓

5e88489...
```

---

# Digital Signature

A Digital Signature verifies:

- Identity
- Integrity
- Authenticity

Uses

- Private Key for Signing
- Public Key for Verification

Applications

- Software Signing
- E-Government Services
- Digital Documents

---

# Digital Certificate

A Digital Certificate is an electronic document that verifies the identity of a person, website, or organization.

Issued By

- Certificate Authority (CA)

Contains

- Public Key
- Owner Information
- Validity Period
- Digital Signature of the CA

---

# SSL/TLS

SSL (deprecated) and TLS are cryptographic protocols that secure communication over the Internet.

Used In

- HTTPS Websites
- Online Banking
- Email Security
- VPN

Benefits

- Encrypts Data
- Protects Privacy
- Prevents Eavesdropping

---

# Common Cryptographic Algorithms

| Algorithm | Type | Common Use |
|-----------|------|------------|
| AES | Symmetric | Data Encryption |
| DES | Symmetric | Legacy Systems |
| 3DES | Symmetric | Legacy Encryption |
| RSA | Asymmetric | Secure Key Exchange |
| ECC | Asymmetric | Mobile Devices |
| SHA-256 | Hash | Password Storage & Integrity |
| SHA-512 | Hash | File Integrity |

---

# Applications of Cryptography

- Online Banking
- ATM Transactions
- Digital Payments
- HTTPS Websites
- VPN
- Secure Email
- Cloud Storage
- Password Protection
- Blockchain
- Digital Signatures

---

# Best Practices

- Use Strong Encryption Algorithms
- Protect Private Keys
- Enable HTTPS
- Avoid Weak Algorithms like MD5 and DES
- Rotate Encryption Keys Regularly
- Store Passwords Using Secure Hashing with Salt
- Keep Cryptographic Libraries Updated

---

# Real-Life Example

When you visit an HTTPS website:

1. Your browser verifies the website's digital certificate.
2. A secure TLS connection is established.
3. Data exchanged between your browser and the website is encrypted.
4. Attackers cannot easily read the transmitted information.

---

# Interview Questions

1. What is Cryptography?
2. What is the difference between Encryption and Decryption?
3. What is Ciphertext?
4. What is the difference between Symmetric and Asymmetric Encryption?
5. What is Hashing?
6. Why is SHA-256 preferred over MD5?
7. What is a Digital Signature?
8. What is a Digital Certificate?
9. What is the purpose of TLS?
10. What are the goals of Cryptography?

---

# Summary

Topics Covered

- Cryptography
- Encryption
- Decryption
- Plaintext
- Ciphertext
- Symmetric Encryption
- Asymmetric Encryption
- Hashing
- Digital Signatures
- Digital Certificates
- SSL/TLS
- Cryptographic Algorithms
- Applications
- Best Practices
- Interview Questions

Cryptography is one of the most important pillars of Cyber Security. It protects sensitive information, secures online communication, and enables trusted digital transactions.

**End of File**
