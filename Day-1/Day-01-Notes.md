# Day 01: Cyber Security Fundamentals & Networking Basics

**Workshop:** 13 Days Cyber Security Workshop  
**Institution:** SJM Institute of Technology (SJMIT College)  

---

## 1. Introduction to Cyber Security

**Cyber Security** is the practice of protecting systems, networks, programs, devices, and data from cyber attacks, unauthorized access, damage, or disruption.

### Core Security Scope
- **Physical Security:** Physical barriers, CCTV monitoring, biometric authentication, facility access control, and disaster management.
- **Software & Network Level Security:** Firewalls, endpoint security, intrusion prevention, encryption, and patch management.
- **The CIA Triad:**
  - **Confidentiality (Privacy):** Ensuring that information is accessible only to authorized personnel.
  - **Integrity:** Maintaining the accuracy, completeness, and trustworthiness of data over its lifecycle.
  - **Availability:** Ensuring timely and reliable access to data and systems for authorized users.

### Common Threat Landscape
- **Viruses & Worms**
- **Malware**
- **Ransomware**
- **Phishing & Social Engineering**

---

## 2. Operating Systems & Server Architectures

### Operating System Types
1. **End-User / Client OS:**
   - Designed for personal computing and everyday tasks.
   - *Examples:* Windows 11, Windows 10, Windows 8.1 / 8, Windows 7, macOS, Desktop Linux distributions.
2. **Server OS:**
   - Optimized for hosting services, handling high concurrency, security policies, and enterprise workloads.
   - *Examples:* Windows Server (2025, 2022, 2019, 2016, 2012), Red Hat Enterprise Linux (RHEL), Ubuntu Server.

### Types of Servers
| # | Server Type | Primary Purpose |
| :--- | :--- | :--- |
| 1 | **Web Server** | Delivers static web content (HTML, CSS, assets) via HTTP/HTTPS (e.g., Apache, Nginx). |
| 2 | **Web Application Server** | Executes dynamic application logic and backend services. |
| 3 | **Database Server** | Stores, manages, and secures structured and unstructured databases. |
| 4 | **Email Server** | Handles incoming and outgoing emails (SMTP, IMAP, POP3). |
| 5 | **Gaming Server** | Manages multiplayer game states and real-time player synchronizations. |
| 6 | **Load Balancer Server** | Distributes incoming client traffic evenly across backend server pools. |
| 7 | **Proxy Server** | Intermediary server that forwards outbound client requests. |
| 8 | **Reverse Proxy Server** | Intermediary server that sits in front of web servers for caching, security, and load distribution. |
| 9 | **Network Server** | Manages network resources, routing, DHCP, and DNS. |
| 10 | **File Server** | Centralized storage for file sharing and access control across a network. |

---

## 3. Domains of Cyber Security

1. **Physical Security:** Securing server rooms, data centers, biometric locks, and surveillance.
2. **Perimeter Security:** Firewalls, perimeter sensors, and boundary defense mechanisms.
3. **Application Security:** Securing software against vulnerabilities like OWASP Top 10 (SQLi, XSS).
4. **Identity & Access Management (IAM):** Role-based access control, multi-factor authentication (MFA), least privilege.
5. **Cloud Security:** Securing public, private, and hybrid cloud infrastructures.
6. **Data Security:** Data encryption (at rest and in transit), data loss prevention (DLP), tokenization.
7. **Email Security:** Anti-phishing, DKIM, SPF, DMARC, spam filters.
8. **AI Security:** Protecting AI/ML models against adversarial attacks and data poisoning.
9. **OS Security:** Hardening operating systems, patch management, kernel protection.
10. **Hardware Security:** Secure boot, TPM chips, hardware security modules (HSM).
11. **Firmware Security:** UEFI/BIOS security, verifying firmware integrity.
12. **Embedded Security:** Microcontroller and embedded systems protection.
13. **Container Security:** Securing Docker images, container runtimes, and Kubernetes clusters.
14. **Network Security:** IDS/IPS, network segmentation, VPNs, and packet filtering.

---

## 4. Specialized Information Security Domains

- **GRC (Governance, Risk, and Compliance):**
  - Frameworks and policies to ensure regulatory adherence (ISO 27001, NIST, SOC 2, HIPAA, GDPR).
- **OT - ICS Security (Operational Technology - Industrial Control Systems):**
  - Protecting critical infrastructure, smart grids, oil & gas pipelines, and heavy manufacturing.
  - *Key Components:* SCADA (Supervisory Control and Data Acquisition), PLC (Programmable Logic Controller), RTU (Remote Terminal Unit).

---

## 5. Ethical Hacking Teams

```text
┌─────────────────────────────────────────────────────────┐
│                   Cyber Security Teams                  │
├──────────────────────────┬──────────────────────────────┤
│ 🔴 Red Team              │ 🔵 Blue Team                 │
│ Offensive Security       │ Defensive Security           │
│ - Penetration Testing    │ - Incident Response          │
│ - Vulnerability Exploit  │ - SOC Monitoring / SIEM      │
│ - Social Engineering     │ - Threat Hunting & Hardening │
├──────────────────────────┴──────────────────────────────┤
│ 🟣 Purple Team: Collaborative unit maximizing feedback  │
│ between Red (attacks) and Blue (defenses)                │
└─────────────────────────────────────────────────────────┘
```

---

## 6. Cyber Security Career Prerequisites

Essential knowledge required for a Cyber Security Engineer:
1. **Operating Systems:** Deep knowledge of Linux and Windows internals.
2. **Networking Fundamentals:** Protocol suites, routing, switching, packet flow.
3. **Scripting & Programming:** Python, Bash, PowerShell for automation and exploit analysis.
4. **Virus & Malware Analysis:** Understanding infection vectors, signature analysis, heuristics.
5. **Core Cybersecurity Principles:** CIA Triad, defence-in-depth, zero-trust architecture.
6. **Databases:** Relational (SQL) and NoSQL architecture and security.
7. **DNS (Domain Name System):** Resolvers, zone transfers, DNS poisoning defense.
8. **Digital Certificates:** Public Key Infrastructure (PKI), SSL/TLS certificates, asymmetric cryptography.
9. **CDN (Content Delivery Network):** Edge caching, DDoS mitigation.
10. **Web Servers & Load Balancing:** Reverse proxies, auto-scaling clusters.

### 📝 Key Question / Assignment
> **Scenario:** *When a user types a URL into a web browser and hits Enter, what exact sequence of events occurs and how does network traffic flow across the infrastructure?*

---

## 7. Networking & The OSI Model

### Definition of Network
A network is a collection of interconnected computers, servers, and electronic devices communicating via transmission media and standardized protocols to share data and resources.

### The 7 Layers of the OSI Model (ISO Standard)
*Developed by the International Organization for Standardization (ISO).*

```text
7. Application Layer   ─── End-user interface (HTTP, HTTPS, FTP, DNS, SSH)
6. Presentation Layer  ─── Data representation, encryption, compression (SSL/TLS, ASCII, JPEG)
5. Session Layer       ─── Manages sessions & dialogues between applications (RPC, NetBIOS)
4. Transport Layer     ─── End-to-end connections & reliability (TCP, UDP, Port numbers)
3. Network Layer       ─── Logical addressing & path determination (IP, ICMP, Routers)
2. Data Link Layer     ─── Physical addressing & error detection (MAC address, Switches)
1. Physical Layer      ─── Raw bit transmission over physical media (Cables, Hubs, Radio waves)
```

---

## 8. IP Addressing Fundamentals (IPv4)

An **IP Address (Internet Protocol)** is a unique 32-bit numeric identifier assigned to every device connected to an IP-based computer network.

### Classes of IPv4 Addresses

| Class | First Octet Range | Default Subnet Mask | Primary Purpose |
| :--- | :--- | :--- | :--- |
| **Class A** | `0 – 126` | `255.0.0.0` (/8) | Very large networks (Enterprise / Telecom) |
| **Class B** | `128 – 191` | `255.255.0.0` (/16) | Medium to large networks (Universities / Corporates) |
| **Class C** | `192 – 223` | `255.255.255.0` (/24) | Small local area networks (Small business / Home) |
| **Class D** | `224 – 239` | N/A | Multicast groups |
| **Class E** | `240 – 255` | N/A | Research, experimental & future use |

*(Note: `127.0.0.0/8` is reserved for loopback and internal diagnostics, e.g., `127.0.0.1` localhost).*

---

## 9. Private IP vs. Public IP Comparison

| Characteristic | Private IP Address | Public IP Address |
| :--- | :--- | :--- |
| **Scope & Usage** | Used only within local networks (LAN) | Used across the global Internet (WAN) |
| **Internet Routability** | Not routable on the public Internet | Globally routable across the public Internet |
| **Assignment** | Configured by local network admin / DHCP router | Assigned by ISP / IANA (Internet Assigned Numbers Authority) |
| **Uniqueness** | Unique only inside the local LAN | Globally unique across the entire world |
| **Cost** | Free of charge | Paid service (provided via ISP subscription) |

### Assigned IP Ranges (RFC 1918)

#### Private IP Ranges
- **Class A:** `10.0.0.0` to `10.255.255.255`
- **Class B:** `172.16.0.0` to `172.31.255.255`
- **Class C:** `192.168.0.0` to `192.168.255.255`

#### Public IP Ranges
- **Class A:** `1.0.0.0` to `9.255.255.255` & `11.0.0.0` to `126.255.255.255`
- **Class B:** `128.0.0.0` to `171.255.255.255` & `172.32.0.0` to `191.255.255.255`
- **Class C:** `192.0.0.0` to `192.167.255.255` & `192.169.0.0` to `223.255.255.255`

---

## 10. Subnet Mask

A **Subnet Mask** is a 32-bit number that separates an IP address into two distinct portions:
1. **Network Bits:** Identifies the specific network address.
2. **Host Bits:** Identifies the specific host device on that network.
