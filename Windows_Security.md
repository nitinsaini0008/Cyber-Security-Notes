# Windows Security

## About

Windows Security is the practice of protecting Microsoft Windows operating systems, user accounts, applications, and data from cyber threats such as malware, unauthorized access, ransomware, and network attacks.

Windows includes several built-in security features that help protect personal computers, enterprise workstations, and Windows Servers.

---

# Why Windows Security is Important

Windows is one of the most widely used operating systems in the world.

Proper security helps to:

- Protect Sensitive Data
- Prevent Malware Infections
- Stop Unauthorized Access
- Reduce Cyber Attacks
- Ensure Business Continuity

---

# Windows Security Features

## 1. Microsoft Defender Antivirus

Microsoft Defender Antivirus provides real-time protection against malware.

Features

- Real-Time Protection
- Virus Detection
- Cloud Protection
- Automatic Updates
- Ransomware Protection

---

## 2. Windows Defender Firewall

Windows Defender Firewall monitors incoming and outgoing network traffic.

Functions

- Allow Trusted Connections
- Block Unauthorized Traffic
- Protect Local Network
- Prevent External Attacks

---

## 3. User Account Control (UAC)

User Account Control prevents unauthorized changes to the system.

Whenever administrative privileges are required, Windows asks for confirmation.

Benefits

- Prevents Unauthorized Software Installation
- Reduces Malware Impact
- Protects System Settings

---

## 4. BitLocker Drive Encryption

BitLocker encrypts the entire disk to protect data if a device is lost or stolen.

Benefits

- Full Disk Encryption
- TPM Support
- Data Protection

---

## 5. Windows Hello

Windows Hello provides passwordless authentication.

Supported Methods

- Fingerprint
- Face Recognition
- PIN

Advantages

- Faster Login
- Improved Security

---

## 6. Microsoft Defender SmartScreen

SmartScreen protects users from:

- Malicious Websites
- Phishing Pages
- Unsafe Downloads

---

# Windows User Accounts

Types of Accounts

## Administrator

- Full Control
- Install Software
- Change System Settings

---

## Standard User

- Limited Permissions
- Safer for Daily Use

---

## Guest Account

- Temporary Access
- Very Limited Permissions

---

# Password Security

Best Practices

- Strong Passwords
- Password Manager
- Enable MFA
- Never Share Passwords
- Lock Computer When Away

---

# Windows Updates

Keeping Windows updated fixes security vulnerabilities.

Settings

```
Settings

↓

Windows Update

↓

Check for Updates
```

Benefits

- Security Patches
- Bug Fixes
- Performance Improvements

---

# Windows Firewall Profiles

| Profile | Usage |
|----------|-------|
| Domain | Organization Network |
| Private | Home Network |
| Public | Public Wi-Fi |

---

# Secure Remote Desktop (RDP)

Remote Desktop allows remote access to Windows systems.

Security Best Practices

- Enable Network Level Authentication (NLA)
- Use Strong Passwords
- Restrict User Access
- Enable MFA
- Change Default RDP Port (Optional)
- Allow Only Trusted IP Addresses

---

# NTFS Permissions

Common NTFS Permissions

- Full Control
- Modify
- Read & Execute
- Read
- Write

NTFS permissions control access to files and folders.

---

# Event Viewer

Event Viewer records system and security events.

Important Logs

- Application Logs
- Security Logs
- System Logs
- Setup Logs

Useful For

- Troubleshooting
- Security Monitoring
- Incident Investigation

---

# Windows Security Tools

| Tool | Purpose |
|------|---------|
| Microsoft Defender | Antivirus |
| Windows Firewall | Network Protection |
| BitLocker | Disk Encryption |
| Event Viewer | Log Monitoring |
| Task Manager | Process Monitoring |
| Windows Security | Central Security Dashboard |
| PowerShell | Administration & Automation |

---

# Common Windows Security Commands

```powershell
whoami
hostname
ipconfig
systeminfo
net user
net localgroup
gpupdate /force
sfc /scannow
DISM /Online /Cleanup-Image /RestoreHealth
```

---

# Common Windows Threats

- Malware
- Ransomware
- Phishing
- Brute Force Attacks
- Privilege Escalation
- USB Malware
- Insider Threats

---

# Best Practices

- Enable Microsoft Defender
- Keep Windows Updated
- Enable Firewall
- Use BitLocker
- Enable MFA
- Use Standard User Accounts
- Backup Important Files
- Disable Unused Services
- Monitor Security Logs
- Install Software Only from Trusted Sources

---

# Real-Life Example

A company uses Windows Server and Windows 11 computers.

Security measures include:

- BitLocker enabled
- Microsoft Defender Antivirus active
- Windows Firewall configured
- Group Policies applied
- MFA for administrator accounts
- Regular Windows Updates

These controls help protect systems against malware, unauthorized access, and data theft.

---

# Interview Questions

1. What is Windows Security?
2. What is Microsoft Defender?
3. What is BitLocker?
4. What is User Account Control (UAC)?
5. What are the Windows Firewall profiles?
6. What is Windows Hello?
7. Why is Event Viewer important?
8. What are NTFS permissions?
9. How can RDP be secured?
10. List five Windows security best practices.

---

# Summary

Topics Covered

- Windows Security
- Microsoft Defender
- Windows Firewall
- UAC
- BitLocker
- Windows Hello
- SmartScreen
- Windows Updates
- NTFS Permissions
- Event Viewer
- PowerShell Commands
- Best Practices
- Interview Questions

Windows Security combines built-in security features, regular updates, strong authentication, encryption, and monitoring to protect systems from modern cyber threats. Following security best practices significantly reduces the risk of attacks.

**End of File**
