# Wireless Security

## About

Wireless Security is the practice of protecting wireless networks (Wi-Fi) from unauthorized access, data theft, and cyber attacks.

Unlike wired networks, wireless communication travels through radio waves, making it easier for attackers within range to intercept or attempt unauthorized access. Proper wireless security helps ensure the confidentiality, integrity, and availability of data.

---

# What is Wireless Security?

Wireless Security includes technologies, protocols, policies, and best practices that protect Wi-Fi networks and connected devices.

It helps protect:

- Home Wi-Fi Networks
- Enterprise Wireless Networks
- Mobile Devices
- IoT Devices
- Wireless Data Communication

---

# Why Wireless Security is Important

Without proper security:

- Attackers can access the network.
- Sensitive data may be intercepted.
- Malware may spread across the network.
- Internet connections may be misused.
- Business operations may be disrupted.

---

# Wireless Security Standards

## 1. WEP (Wired Equivalent Privacy)

### Features

- First Wi-Fi security standard
- Uses RC4 encryption

### Disadvantages

- Weak encryption
- Easily cracked
- No longer recommended

---

## 2. WPA (Wi-Fi Protected Access)

### Features

- Improved security over WEP
- Introduced TKIP encryption

### Advantages

- Better than WEP

### Disadvantages

- Considered outdated

---

## 3. WPA2

### Features

- Uses AES encryption
- Widely supported

### Advantages

- Strong security
- Stable
- Suitable for most environments

---

## 4. WPA3

### Features

- Latest Wi-Fi security standard
- Stronger authentication
- Improved encryption

### Advantages

- Better protection against password attacks
- Improved privacy
- Recommended for new networks

---

# Comparison Table

| Standard | Encryption | Security Level |
|-----------|------------|----------------|
| WEP | RC4 | Very Low |
| WPA | TKIP | Low |
| WPA2 | AES | High |
| WPA3 | AES with improved authentication | Very High |

---

# Common Wireless Attacks

## 1. Evil Twin Attack

An attacker creates a fake Wi-Fi access point that looks like a legitimate network.

Purpose

- Steal Login Credentials
- Capture Network Traffic

---

## 2. Rogue Access Point

An unauthorized wireless access point connected to an organization's network.

Risk

- Unauthorized Access
- Data Theft

---

## 3. Packet Sniffing

Attackers capture wireless traffic to analyze or steal information.

Prevention

- Use WPA2/WPA3
- Enable HTTPS
- Use VPN on public Wi-Fi

---

## 4. Deauthentication Attack

Attackers send fake deauthentication frames to disconnect users from a Wi-Fi network.

Purpose

- Denial of Service
- Force Reconnection
- Capture Authentication Handshakes

---

## 5. Brute Force Attack

Attackers repeatedly guess Wi-Fi passwords.

Prevention

- Long Passwords
- WPA3
- Disable Weak Security Protocols

---

# Secure Wi-Fi Configuration

- Use WPA3 whenever possible.
- If WPA3 is unavailable, use WPA2 with AES.
- Disable WEP and WPA.
- Create a strong Wi-Fi password.
- Change default administrator credentials.
- Update router firmware regularly.

---

# Guest Wi-Fi Network

Organizations should provide a separate guest network.

Benefits

- Isolates Guest Devices
- Protects Internal Resources
- Reduces Security Risks

---

# MAC Address Filtering

Routers can allow only approved device MAC addresses.

Advantages

- Additional Security Layer

Limitations

- MAC addresses can be spoofed
- Should not be the only security control

---

# Disable WPS

Wi-Fi Protected Setup (WPS) makes connecting devices easier but can introduce security risks.

Recommendation

- Disable WPS unless there is a specific need.

---

# Wireless Network Monitoring

Monitor for:

- Unknown Devices
- Rogue Access Points
- Unusual Traffic
- Authentication Failures
- Signal Interference

Tools

- Wireshark
- Kismet
- Aircrack-ng (for authorized security testing)
- NetSpot

---

# Best Practices

- Use WPA3 or WPA2-AES
- Use Strong Wi-Fi Passwords
- Change Default Router Credentials
- Keep Router Firmware Updated
- Disable WPS
- Enable Guest Networks
- Use VPN on Public Wi-Fi
- Monitor Connected Devices
- Review Router Logs Regularly

---

# Real-Life Example

A company configures its wireless network using:

- WPA3 Encryption
- Strong Administrator Password
- Separate Guest Wi-Fi
- Updated Router Firmware
- Continuous Wireless Monitoring

These controls help protect the organization's wireless network from unauthorized access and common Wi-Fi attacks.

---

# Interview Questions

1. What is Wireless Security?
2. Why is WEP considered insecure?
3. What is the difference between WPA2 and WPA3?
4. What is an Evil Twin attack?
5. What is a Rogue Access Point?
6. Why should WPS be disabled?
7. What is MAC Address Filtering?
8. Why should guest Wi-Fi be separated from the main network?
9. Name three wireless security best practices.
10. Which Wi-Fi security standard is recommended today?

---

# Summary

Topics Covered

- Wireless Security
- WEP
- WPA
- WPA2
- WPA3
- Evil Twin Attack
- Rogue Access Point
- Packet Sniffing
- Deauthentication Attack
- Brute Force Attack
- Guest Networks
- MAC Address Filtering
- WPS
- Wireless Monitoring
- Best Practices
- Interview Questions

Wireless Security is essential for protecting Wi-Fi networks from unauthorized access and cyber threats. Using WPA3, strong passwords, updated firmware, secure configurations, and continuous monitoring greatly improves the security of wireless environments.

**End of File**
