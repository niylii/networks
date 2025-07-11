# Network Security Summary

This document provides a concise yet comprehensive overview of computer networks in the context of cybersecurity. It outlines core concepts, common vulnerabilities, attack techniques, and modern defense strategies, with references to tools and practices widely used in the industry.

---

##  What is a Network?

A **computer network** is a group of interconnected devices that communicate using specific protocols and transmission technologies. In cybersecurity, networks are both critical assets to protect and potential attack surfaces to exploit.

---

##  The OSI Model in Security Context

Understanding the **OSI (Open Systems Interconnection)** model is essential for identifying vulnerabilities and applying effective defenses at each layer:

| Layer | Name           | Security Focus                                   |
|-------|----------------|--------------------------------------------------|
| 1     | Physical        | Wiretapping, hardware keyloggers, signal jamming |
| 2     | Data Link       | MAC spoofing, ARP poisoning                      |
| 3     | Network         | IP spoofing, DDoS attacks, routing manipulation  |
| 4     | Transport       | Port scanning, TCP SYN floods                    |
| 5     | Session         | Session hijacking, replay attacks                |
| 6     | Presentation    | SSL stripping, data tampering                    |
| 7     | Application     | XSS, SQL injection, DNS attacks, API exploitation|

---

##  Core Network Security Concepts

- **Firewall:** Filters traffic based on rules (stateless/stateful)
- **IDS/IPS:** Detects and/or blocks malicious activity
- **VPNs:** Encrypt data over insecure networks
- **Network Segmentation:** Limits the scope of compromise
- **ACLs (Access Control Lists):** Define who can access what
- **Zero Trust Architecture:** Trust no one by default, verify everything
- **Authentication Protocols:** 802.1X, RADIUS, TACACS+ (did'nt get to that one yet...)

---

## Common Network Attacks

- **Man-in-the-Middle (MITM):** Intercept and manipulate communications
- **ARP Spoofing:** Redirect traffic by impersonating MAC addresses
- **DDoS Attacks:** Overwhelm a system with massive traffic
- **DNS Spoofing:** Redirect users to malicious websites
- **Packet Sniffing:** Intercept unencrypted data in transit
- **Session Hijacking:** Take control of active sessions
- **Port Scanning:** Identify open services and potential entry points

---

##  Essential Tools

| Tool        | Purpose                       |
|-------------|-------------------------------|
| `nmap`      | Network scanning and mapping  |
| `wireshark` | Packet capture and analysis   |
| `netcat`    | Reading/writing data over TCP/UDP |
| `tcpdump`   | Command-line packet analysis  |
| `ettercap`  | MITM attacks and sniffing     |
| `arpspoof`  | ARP spoofing for MITM         |
| `aircrack-ng` | Wireless network exploitation |
| `traceroute`, `dig` | Network diagnostics     |

---

##  Defense Strategies

- **Encryption:** Secure communication using TLS, IPsec, etc.
- **Monitoring & Logging:** SIEM tools (e.g., Splunk, ELK) to detect anomalies
- **Patch Management:** Regularly update systems and devices
- **Access Control:** Principle of least privilege (PoLP)
- **User Awareness Training:** Prevent social engineering and phishing
- **Threat Hunting:** Proactive detection of anomalies and Indicators of Compromise (IOCs)

---
## ✅ Summary

Network security is an evolving discipline that combines **technical controls**, **policy enforcement**, and **constant vigilance**. From low-level hardware to high-level applications, each layer presents risks and opportunities for defense. Mastery of networking fundamentals is a core skill for any cybersecurity professional.

---
