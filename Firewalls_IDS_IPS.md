# Firewalls, IDS & IPS

## About

Firewalls, Intrusion Detection Systems (IDS), and Intrusion Prevention Systems (IPS) are essential components of network security. They help protect networks from unauthorized access, monitor suspicious activities, and stop cyber attacks before they cause damage.

---

# Firewall

## Definition

A Firewall is a network security device or software that monitors and controls incoming and outgoing network traffic based on predefined security rules.

It acts as a barrier between a trusted internal network and an untrusted external network such as the Internet.

---

# How a Firewall Works

```
Internet
    │
    ▼
+-----------+
| Firewall  |
+-----------+
    │
    ▼
Internal Network
```

The firewall checks every packet and decides whether to:

- Allow
- Block
- Reject
- Log

---

# Types of Firewalls

## 1. Packet Filtering Firewall

Examines packet headers such as:

- Source IP
- Destination IP
- Protocol
- Port Number

Advantages

- Fast
- Simple
- Low Resource Usage

Disadvantages

- Limited Security
- Cannot Inspect Packet Content

---

## 2. Stateful Firewall

Tracks active network connections and allows only packets belonging to valid sessions.

Advantages

- Better Security
- Tracks Connections

Disadvantages

- Higher Resource Usage

---

## 3. Proxy Firewall

Acts as an intermediary between users and servers.

Advantages

- Hides Internal Network
- Content Filtering
- Better Privacy

Disadvantages

- Slightly Slower

---

## 4. Next-Generation Firewall (NGFW)

Combines traditional firewall capabilities with advanced security features.

Features

- Deep Packet Inspection
- Application Awareness
- Malware Detection
- Intrusion Prevention
- SSL Inspection

---

# Firewall Rules

Examples

Allow

```
Allow TCP Port 80 (HTTP)
Allow TCP Port 443 (HTTPS)
Allow SSH from Admin IP Only
```

Block

```
Block Telnet
Block Unknown Ports
Block Suspicious IP Addresses
```

---

# Intrusion Detection System (IDS)

## Definition

An IDS monitors network or host activity and detects suspicious behavior or known attack patterns.

Unlike an IPS, an IDS only detects and alerts—it does not automatically block attacks.

---

# Types of IDS

## 1. Network IDS (NIDS)

Monitors traffic flowing through a network.

Examples

- Snort
- Suricata
- Zeek

---

## 2. Host IDS (HIDS)

Monitors activities on an individual computer or server.

Examples

- OSSEC
- Wazuh

---

# IDS Detection Methods

## Signature-Based Detection

Detects known attacks using predefined signatures.

Advantages

- Accurate for Known Threats

Disadvantages

- Cannot Detect Unknown Attacks

---

## Anomaly-Based Detection

Detects unusual behavior compared to normal activity.

Advantages

- Can Detect New Threats

Disadvantages

- May Produce False Positives

---

# Intrusion Prevention System (IPS)

## Definition

An IPS monitors network traffic and automatically blocks or prevents malicious activity in real time.

Unlike IDS, IPS can actively stop attacks.

---

# IPS Functions

- Detect Threats
- Block Malicious Packets
- Reset Connections
- Generate Security Alerts
- Log Security Events

---

# Types of IPS

## 1. Network IPS (NIPS)

Protects the entire network by monitoring traffic.

---

## 2. Host IPS (HIPS)

Protects a specific computer or server.

---

## 3. Wireless IPS (WIPS)

Protects wireless networks against attacks.

---

# IDS vs IPS

| Feature | IDS | IPS |
|---------|-----|-----|
| Detects Threats | Yes | Yes |
| Blocks Attacks | No | Yes |
| Generates Alerts | Yes | Yes |
| Inline Deployment | No | Yes |
| Prevents Attacks Automatically | No | Yes |

---

# Firewall vs IDS vs IPS

| Feature | Firewall | IDS | IPS |
|---------|----------|-----|-----|
| Filters Traffic | Yes | No | Yes |
| Detects Attacks | Limited | Yes | Yes |
| Blocks Attacks | Yes | No | Yes |
| Monitors Network | Limited | Yes | Yes |
| Uses Security Rules | Yes | Yes | Yes |

---

# Popular Security Tools

## Firewalls

- pfSense
- Cisco ASA
- FortiGate
- Palo Alto Networks
- Check Point

---

## IDS/IPS

- Snort
- Suricata
- Zeek
- Wazuh
- OSSEC

---

# Best Practices

- Keep Firewall Rules Updated
- Block Unused Ports
- Enable Logging
- Deploy IDS and IPS Together
- Monitor Alerts Regularly
- Update Security Signatures
- Use the Principle of Least Privilege
- Review Firewall Policies Periodically

---

# Real-Life Example

A company hosts a public web server.

Security measures include:

- Firewall allows only HTTP (80) and HTTPS (443).
- IDS monitors traffic for suspicious behavior.
- IPS automatically blocks malicious requests and known attack patterns.

Together, these technologies provide layered network protection.

---

# Advantages

- Prevent Unauthorized Access
- Detect Malicious Activity
- Automatically Block Attacks
- Improve Network Visibility
- Strengthen Overall Security

---

# Limitations

- Incorrect Rules Can Block Legitimate Traffic
- Signature-Based Detection Misses Unknown Threats
- False Positives May Occur
- Regular Updates and Monitoring Are Required

---

# Interview Questions

1. What is a Firewall?
2. What is the difference between IDS and IPS?
3. What are the types of Firewalls?
4. What is a Stateful Firewall?
5. What is a Network IDS?
6. What is a Host IPS?
7. What is Signature-Based Detection?
8. What is Anomaly-Based Detection?
9. Why are Firewalls, IDS, and IPS used together?
10. Name three popular IDS/IPS tools.

---

# Summary

Topics Covered

- Firewall
- Types of Firewalls
- Firewall Rules
- IDS
- IPS
- IDS Detection Methods
- Types of IPS
- Firewall vs IDS vs IPS
- Security Tools
- Best Practices
- Interview Questions

Firewalls, IDS, and IPS form a layered defense strategy. Firewalls filter traffic, IDS detects suspicious activities, and IPS actively blocks threats, providing comprehensive protection for modern networks.

**End of File**
