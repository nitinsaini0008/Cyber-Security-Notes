# Linux Security

## About

Linux Security is the practice of protecting Linux operating systems, servers, applications, and data from unauthorized access, malware, and cyber attacks.

Linux is widely used in servers, cloud computing, networking, DevOps, and cyber security because of its stability, flexibility, and strong security features.

---

# Why Linux Security is Important

Linux systems often host:

- Web Servers
- Database Servers
- Cloud Infrastructure
- Enterprise Applications
- Network Services

A compromised Linux server can expose sensitive data and disrupt business operations.

---

# Linux Security Principles

- Least Privilege
- Defense in Depth
- Secure Configuration
- Regular Updates
- Continuous Monitoring

---

# User and Group Security

Linux controls access using users and groups.

## Types of Users

### Root User

- Full administrative privileges
- User ID (UID): 0

### Normal User

- Limited permissions
- Cannot modify system files without authorization

### System User

- Used by services and applications
- Usually cannot log in interactively

---

# File Permissions

Linux permissions determine who can read, write, or execute files.

Example

```
-rwxr-xr--
```

Permission Meaning

| Permission | Meaning |
|------------|---------|
| r | Read |
| w | Write |
| x | Execute |
| - | No Permission |

Permission Categories

- Owner
- Group
- Others

---

# Numeric Permissions

| Number | Permission |
|---------|------------|
| 7 | rwx |
| 6 | rw- |
| 5 | r-x |
| 4 | r-- |
| 0 | --- |

Example

```
chmod 755 file.sh
```

---

# File Ownership

Useful Commands

```bash
ls -l
chown user file.txt
chgrp group file.txt
```

---

# Sudo

`sudo` allows authorized users to execute administrative commands without logging in directly as the root user.

Example

```bash
sudo apt update
```

Benefits

- Better Accountability
- Reduced Risk
- Controlled Administrative Access

---

# Password Security

Best Practices

- Strong Passwords
- Password Expiration Policies
- Password Complexity
- MFA (where supported)

Useful Commands

```bash
passwd
chage
```

---

# SSH Security

SSH provides secure remote access to Linux systems.

Best Practices

- Disable Root Login
- Use SSH Keys
- Disable Password Authentication (where practical)
- Change the Default Port (optional)
- Enable MFA if available

Useful File

```
/etc/ssh/sshd_config
```

---

# Firewall

Popular Linux Firewalls

- UFW
- firewalld
- iptables
- nftables

Example

```bash
sudo ufw enable
```

Check Status

```bash
sudo ufw status
```

---

# Software Updates

Keep packages updated to reduce security risks.

Ubuntu/Debian

```bash
sudo apt update
sudo apt upgrade
```

Red Hat/Rocky/AlmaLinux

```bash
sudo dnf update
```

---

# Malware Protection

Although Linux is generally less targeted than desktop operating systems, it can still be affected by malware.

Popular Tools

- ClamAV
- Linux Malware Detect (LMD)

---

# Log Monitoring

Important Log Files

| Log File | Purpose |
|----------|---------|
| /var/log/auth.log | Authentication Logs (Debian/Ubuntu) |
| /var/log/secure | Authentication Logs (RHEL-based) |
| /var/log/syslog | System Logs |
| /var/log/messages | General System Logs |
| /var/log/dmesg | Kernel Messages |

Useful Commands

```bash
tail
less
journalctl
grep
```

---

# Disk Encryption

Disk encryption protects data if a storage device is lost or stolen.

Common Technology

- LUKS (Linux Unified Key Setup)

---

# Backup

Regular backups help recover from accidental deletion, hardware failure, or ransomware.

Backup Methods

- Local Backup
- External Drive
- Cloud Backup

Popular Tools

- rsync
- tar
- BorgBackup

---

# SELinux and AppArmor

## SELinux

Mandatory Access Control (MAC) framework commonly used in Red Hat Enterprise Linux.

Modes

- Enforcing
- Permissive
- Disabled

Useful Command

```bash
getenforce
```

---

## AppArmor

Application-level security framework commonly used in Ubuntu.

Benefits

- Restricts Application Capabilities
- Improves System Security

---

# Common Linux Security Commands

```bash
whoami
id
passwd
chmod
chown
groups
sudo
ufw status
ss -tuln
ps aux
top
journalctl
last
```

---

# Best Practices

- Keep Systems Updated
- Use Strong Passwords
- Disable Unused Services
- Use SSH Keys
- Enable Firewalls
- Monitor Logs
- Limit Root Access
- Backup Important Data
- Apply the Principle of Least Privilege
- Perform Regular Security Audits

---

# Real-Life Example

A company hosts its website on an Ubuntu server.

Security measures include:

- SSH key-based authentication
- UFW firewall enabled
- Automatic security updates
- Regular log monitoring
- Daily encrypted backups

These controls help protect the server against unauthorized access and common attacks.

---

# Interview Questions

1. What is Linux Security?
2. Why should direct root login be avoided?
3. What do the permissions `755` and `644` mean?
4. What is the purpose of `sudo`?
5. What is UFW?
6. What is SELinux?
7. What is AppArmor?
8. Which command changes file permissions?
9. Why are log files important?
10. List five Linux security best practices.

---

# Summary

Topics Covered

- Linux Security
- Users and Groups
- File Permissions
- File Ownership
- Sudo
- Password Security
- SSH Security
- Firewalls
- Software Updates
- Malware Protection
- Log Monitoring
- Disk Encryption
- Backups
- SELinux
- AppArmor
- Best Practices
- Interview Questions

Linux Security is a critical part of protecting servers and enterprise systems. Proper user management, secure configurations, regular updates, firewalls, and continuous monitoring greatly reduce the risk of security incidents.

**End of File**
