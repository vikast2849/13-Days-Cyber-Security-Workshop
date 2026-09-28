# Day 02: Advanced Networking, Operating Systems & Cloud Fundamentals

**Workshop:** 13 Days Cyber Security Workshop  
**Institution:** SJM Institute of Technology (SJMIT College)  

---

## 1. Advanced Networking Concepts

### Subnetting
**Subnetting** is the process of partitioning a single large physical or logical network into multiple smaller, distinct subnetworks (subnets).
- **Benefits:** Minimizes broadcast traffic, improves network performance, enables granular access control, and conserves IP addresses.

### Supernetting
**Supernetting** (Classless Inter-Domain Routing / CIDR Aggregation) is the process of combining multiple contiguous smaller network blocks into a single larger network address prefix.
- **Benefits:** Drastically reduces the size and overhead of router routing tables.

### Routing & Protocols
- **Routing:** The systematic mechanism of selecting the best path across one or more networks to deliver data packets from a source to a destination.
- **Network Protocol:** A standardized set of rules and conventions governing how devices format, transmit, verify, and receive data.

### Common Routing Protocols
| Protocol | Full Name | Type | Description |
| :--- | :--- | :--- | :--- |
| **RIP v1** | Routing Information Protocol (v1) | Distance Vector (Classful) | Legacy routing protocol utilizing hop count as its metric (max 15 hops). |
| **RIP v2** | Routing Information Protocol (v2) | Distance Vector (Classless) | Upgraded version supporting CIDR and subnet masks. |
| **EIGRP** | Enhanced Interior Gateway Routing Protocol | Advanced Distance Vector / Hybrid | Cisco proprietary protocol offering fast convergence and low bandwidth usage. |
| **IGRP** | Interior Gateway Routing Protocol | Distance Vector (Classful) | Cisco legacy interior gateway protocol (superseded by EIGRP). |
| **BGP** | Border Gateway Protocol | Path Vector | The core routing protocol of the global Internet, routing between Autonomous Systems (AS). |

---

## 2. Port Numbers & Categories

A **Port Number** is a 16-bit unsigned integer (ranging from `0` to `65535`) that serves as a logical communication endpoint in an operating system, identifying specific network services or processes.

### Port Ranges (IANA Standard)

| Port Range | Category | Purpose & Description |
| :--- | :--- | :--- |
| **`0 – 1023`** | **Well-Known Ports** | Reserved for standard system services and core Internet protocols (e.g., HTTP: `80`, HTTPS: `443`, SSH: `22`, DNS: `53`, FTP: `20/21`). |
| **`1024 – 49151`** | **Registered Ports** | Assigned by IANA for specific vendor applications and user-level processes (e.g., MySQL: `3306`, RDP: `3389`, PostgreSQL: `5432`). |
| **`49152 – 65535`** | **Dynamic / Private / Ephemeral Ports** | Temporary ports automatically assigned by the client OS to manage outbound connections during communication sessions. |

---

## 3. Web State & Memory Concepts

- **Cookies:** Small pieces of data stored on the client’s browser by web servers to track state, personalization, and user sessions.
- **Sessions:** Server-side mechanisms that securely maintain user state and authentication information across multiple HTTP requests.
- **Cache:** High-speed temporary memory storage used to store frequently accessed data and reduce retrieval latency.
- **Buffer:** A temporary region of physical RAM used to hold data while it is being transferred between devices or processes.

---

## 4. Operating System Architecture & Management

An Operating System (OS) manages computer hardware, system software, and shared resources.

### Core Management Modules of an OS
1. **Process Management:** CPU scheduling, process creation, execution, synchronization, and termination.
2. **Service / Daemon Management:** Managing background system services (systemd, Windows services).
3. **Memory Management:** Tracking memory locations, paging, segmentation, and virtual memory allocation.
4. **File System Management:** Structuring files, directory hierarchies, permissions, and disk storage.
5. **User & Identity Management:** Managing user accounts, groups, authentication, and access rights.
6. **Security Management:** Antivirus integration, firewall policies, access control lists (ACLs).
7. **Scripting & Automation:** Executing shell scripts, batch files, and scheduled tasks (cron, Task Scheduler).
8. **Network Management:** Socket handling, network interface configuration, and traffic routing.
9. **Server Management:** Resource balancing, multi-user concurrency, and high-availability operations.
10. **Troubleshooting & Diagnostics:** Event logs, kernel dumps, performance profiling, and error analysis.

### OS Core Components
- **Kernel:** The foundational core of the OS that directly interacts with the hardware (CPU, RAM, devices).
- **Shell:** The user interface (CLI/GUI) that translates commands into kernel operations.
- **Interpreter:** Translates and executes script instructions line-by-line in real time.
- **Compiler:** Translates high-level source code into native machine code.
- **Hardware:** Physical devices (Processor, Memory, Motherboard, I/O devices).

### OS Boot Sequences
- **Windows Boot Flow:** BIOS/UEFI → Master Boot Record (MBR)/GPT → Windows Boot Manager → `winload.efi` → NT Kernel (`ntoskrnl.exe`) → HAL → System Services (`smss.exe`) → Logon Screen (`winlogon.exe`).
- **Linux Boot Flow:** BIOS/UEFI → GRUB Bootloader → Kernel Initialization → `initramfs` → `systemd` (PID 1) → Default Target / Multi-user Runlevel.

---

## 5. Linux Distribution Families

```text
┌──────────────────────────────────────────────────────────────┐
│                  Linux Distribution Families                 │
├──────────────────────────────┬───────────────────────────────┤
│ 🔴 Red Hat Family            │ 🔵 Debian Family              │
│ - Red Hat Enterprise Linux   │ - Debian                      │
│ - CentOS                     │ - Ubuntu                      │
│ - Fedora                     │ - Kali Linux (Security / Pen) │
│ - Package Manager: RPM / DNF │ - Linux Mint                  │
│                              │ - Package Manager: DPKG / APT │
└──────────────────────────────┴───────────────────────────────┘
```

---

## 6. Remote Operating System Connectivity Matrix

| Source (Client) | Destination (Host) | Protocol | Port & Transport | Primary Tools / Clients |
| :--- | :--- | :--- | :--- | :--- |
| **Windows** | **Linux** | **SSH** | `22 / TCP` | PuTTY, Windows Terminal, OpenSSH, PowerShell |
| **Windows** | **Windows** | **RDP** | `3389 / TCP` | Remote Desktop Connection (`mstsc`), PowerShell Remoting |
| **Windows** | **Windows (Mgmt)** | **WinRM** | `5985 (HTTP) / 5986 (HTTPS)` | PowerShell Remoting, Windows Admin Center |
| **Windows** | **macOS** | **SSH / VNC** | `22 / 5900 TCP` | PuTTY, VNC Viewer, Screen Sharing |
| **macOS** | **Linux** | **SSH** | `22 / TCP` | macOS Terminal, OpenSSH |
| **macOS** | **Windows** | **RDP** | `3389 / TCP` | Microsoft Remote Desktop for Mac |
| **Linux** | **Linux** | **SSH** | `22 / TCP` | Linux Terminal, OpenSSH |
| **Linux** | **Windows** | **RDP** | `3389 / TCP` | Remmina, FreeRDP, rdesktop |

---

## 7. Linux Shells & CLI Environments

A **Shell** is a command language interpreter that executes commands entered by the user or read from scripts, interfacing with the Linux kernel.

| Shell | Full Name | Key Features & Primary Use Case |
| :--- | :--- | :--- |
| **`bash`** | Bourne Again Shell | The standard default general-purpose shell on most Linux distributions; excellent for shell scripting. |
| **`sh`** | Bourne Shell | The original UNIX shell; lightweight and standard for POSIX compatibility scripts. |
| **`zsh`** | Z Shell | Advanced interactive shell; highly customizable with plugins, themes (Oh-My-Zsh), and advanced auto-completion. |
| **`fish`** | Friendly Interactive Shell | Modern out-of-the-box user-friendly shell with auto-suggestions, syntax highlighting, and web-based configuration. |
| **`ksh`** | Korn Shell | Combines features of the C shell and Bourne shell; popular in enterprise UNIX environments. |
| **`tcsh` / `csh`** | C Shell / TENEX C Shell | Utilizes a C-like programming language syntax for scripting and interactive sessions. |
| **`dash`** | Debian Almquist Shell | Extremely lightweight and fast POSIX-compliant shell; used in Debian/Ubuntu for system initialization scripts. |

---

## 8. Cloud Computing Fundamentals

**Cloud Computing** is the on-demand delivery of IT infrastructure and services over the Internet with pay-as-you-go pricing.

### Major Cloud Service Providers

| Domain | Amazon Web Services (AWS) | Microsoft Azure | Google Cloud Platform (GCP) |
| :--- | :--- | :--- | :--- |
| **Compute / Virtual Machines** | EC2 (Elastic Compute Cloud) | Azure Virtual Machines | Compute Engine |
| **Object Storage** | S3 (Simple Storage Service) | Azure Blob Storage | Cloud Storage |
| **Resource Nomenclature** | Services & Resources | Resources & Resource Groups | APIs & Projects |

### AWS Global Infrastructure
- **Regions (26+ Worldwide):** Physical geographic locations around the world where data centers are clustered.
- **Availability Zones (AZs):**
  - Each AWS Region contains a minimum of **3** and up to **6** Availability Zones.
  - Each AZ consists of one or more discrete data centers with redundant power, networking, and connectivity.
  - AZs within a region are interconnected with high-bandwidth, ultra-low-latency networking.

### Key Factors for Selecting a Cloud Region
1. **Latency & Proximity:** Placing resources geographically close to end users to reduce response times.
2. **Service Availability:** Ensuring specific cloud services and instance types are offered in that region.
3. **Compliance & Legal Governance:** Adhering to local data sovereignty laws (e.g., GDPR, HIPAA).
4. **Cost & Pricing:** Resource pricing varies across regions due to taxes, infrastructure, and operating costs.
