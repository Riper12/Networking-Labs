# Networking Support & Troubleshooting Labs

## 📌 Overview

This repository contains my **hands-on networking labs** created to practice and demonstrate practical skills required for **Network Support Engineer, IT Support, Technical Support, Service Desk, and IT Technician** roles.

The labs focus on understanding and troubleshooting common networking issues using **Cisco Packet Tracer, Windows networking tools, Linux, and network troubleshooting methodologies**.

Each lab is documented in a ticket-style format with:

* Problem statement
* Network topology
* Configuration steps
* Commands used
* Troubleshooting process
* Expected results
* Actual results
* Root cause
* Resolution
* Verification
* Screenshots/evidence

The goal is to build **practical, job-oriented networking troubleshooting skills** and maintain a documented proof-of-work portfolio.

---

# 🧰 Tools & Technologies

| Tool / Technology   | Purpose                               |
| ------------------- | ------------------------------------- |
| Cisco Packet Tracer | Network simulation and configuration  |
| Windows 10/11       | Client-side troubleshooting           |
| Linux / Ubuntu      | Linux networking and troubleshooting  |
| Kali Linux          | Network diagnostic and security tools |
| Wireshark           | Packet capture and traffic analysis   |
| Nmap                | Network discovery and port scanning   |
| VS Code             | Documentation and configuration files |
| Git & GitHub        | Version control and portfolio         |

---

# 🌐 Networking Concepts Covered

The labs cover the following networking concepts:

### Network Fundamentals

* OSI Model
* TCP/IP Model
* IPv4 addressing
* Subnet masks
* Default gateway
* MAC addresses
* ARP
* Broadcast and unicast
* LAN / WAN
* Network interfaces
* Common networking ports and protocols

### IP Networking

* Static IP configuration
* DHCP
* DNS
* IPv4 subnetting
* Default gateway
* Network and host identification
* Private IP addressing
* APIPA
* IP address troubleshooting

### Switching

* Cisco switch configuration
* VLANs
* Access ports
* Trunk ports
* MAC address table
* Port status
* Basic switch security
* Switch troubleshooting

### Routing

* Router configuration
* Router interfaces
* Inter-network communication
* Routing table
* Static routing
* Default routes
* Router troubleshooting

### Network Troubleshooting

* `ping`
* `tracert` / `traceroute`
* `ipconfig`
* `ip`
* `ifconfig`
* `nslookup`
* `arp`
* `netstat`
* `route`
* `ipconfig /flushdns`
* `ipconfig /release`
* `ipconfig /renew`

### Network Services

* DHCP
* DNS
* HTTP / HTTPS
* SSH
* FTP
* ICMP
* TCP
* UDP

---

# 🧪 Lab Structure

Each networking scenario is organized as an individual lab.

Example:

```text
Networking-Labs/
│
├── 01-Small-LAN-Ping-Troubleshooting/
│   ├── README.md
│   ├── Screenshots/
│   └── Ticket.md
│
├── 02-Cisco-Switch-Basic-Configuration/
│   ├── README.md
│   ├── Screenshots/
│   └── Ticket.md
│
├── 03-VLAN-Configuration/
│   ├── README.md
│   ├── Screenshots/
│   └── Ticket.md
│
├── 04-Router-Configuration/
│   ├── README.md
│   ├── Screenshots/
│   └── Ticket.md
│
├── 05-DHCP-Troubleshooting/
│   ├── README.md
│   ├── Screenshots/
│   └── Ticket.md
│
└── 06-DNS-Troubleshooting/
    ├── README.md
    ├── Screenshots/
    └── Ticket.md
```

---

# 🎫 Troubleshooting Methodology

The labs follow a structured IT support troubleshooting approach.

### Step 1 — Identify the Problem

Understand the reported issue and collect information from the user or monitoring system.

Example:

> User cannot access another computer on the network.

---

### Step 2 — Gather Information

Check:

* IP address
* Subnet mask
* Default gateway
* DNS configuration
* Network adapter status
* Physical connectivity
* Link status
* VLAN assignment

---

### Step 3 — Test Connectivity

Use appropriate troubleshooting commands.

Windows:

```powershell
ipconfig
ping <IP-address>
tracert <IP-address>
nslookup <domain>
arp -a
```

Linux:

```bash
ip addr
ip route
ping <IP-address>
traceroute <IP-address>
nslookup <domain>
arp -a
```

Cisco:

```text
show ip interface brief
show ip route
show vlan brief
show interfaces
show mac address-table
```

---

### Step 4 — Isolate the Fault

Determine whether the issue is related to:

* Physical connectivity
* Client configuration
* IP addressing
* VLAN
* Switch
* Router
* DHCP
* DNS
* Firewall
* Routing
* Application/service

---

### Step 5 — Apply the Fix

Make the required configuration or corrective action.

Examples:

* Correct an incorrect IP address
* Enable a disabled interface
* Correct VLAN assignment
* Configure a missing default gateway
* Renew DHCP lease
* Flush DNS cache
* Correct router configuration
* Replace faulty network cable

---

### Step 6 — Verify the Resolution

Repeat the appropriate tests to confirm that the problem has been resolved.

Example:

```text
PC1 → ping PC2
PC1 → ping Default Gateway
PC1 → ping DNS Server
PC1 → nslookup example.com
```

---

### Step 7 — Document the Resolution

Record:

* Root cause
* Troubleshooting performed
* Corrective action
* Verification result
* Lessons learned

---

# 📚 Current Lab Progress

| Lab | Scenario                             | Status         |
| --- | ------------------------------------ | -------------- |
| 01  | Small LAN – PC to PC Connectivity    | 🟡 In Progress |
| 02  | Cisco Switch Basic Configuration     | 🟡 In Progress |
| 03  | VLAN Configuration                   | ⬜ Planned      |
| 04  | Router Interface Configuration       | ⬜ Planned      |
| 05  | Inter-Network Routing                | ⬜ Planned      |
| 06  | DHCP Troubleshooting                 | ⬜ Planned      |
| 07  | DNS Troubleshooting                  | ⬜ Planned      |
| 08  | Network Connectivity Troubleshooting | ⬜ Planned      |
| 09  | Wireshark Packet Analysis            | ⬜ Planned      |
| 10  | Nmap Network Discovery               | ⬜ Planned      |

> Lab status will be updated as each scenario is completed and documented with my own screenshots and testing evidence.

---

# 🖥️ Example Network Topology

Basic LAN:

```text
        PC1
    192.168.1.10
         |
         |
      [Switch]
         |
         |
        PC2
    192.168.1.20
```

Example routed network:

```text
     Network 1
  192.168.1.0/24
        |
       PC1
        |
     [Switch]
        |
        |
     [Router]
        |
        |
     [Switch]
        |
       PC2
        |
  192.168.2.0/24
     Network 2
```

---

# 🔍 Evidence & Documentation

Screenshots are included for important configuration and verification steps.

Evidence may include:

* Packet Tracer topology
* Cisco CLI configuration
* IP configuration
* Ping results
* Traceroute results
* VLAN configuration
* Routing table
* Interface status
* Wireshark packet captures
* Nmap scan results
* Troubleshooting before/after results

Example:

```markdown
![Network Topology](Screenshots/network-topology.png)
```

---

# 🧠 Skills Demonstrated

Through these labs, I am developing practical experience in:

* Network troubleshooting
* TCP/IP fundamentals
* IPv4 addressing
* Subnetting
* DNS troubleshooting
* DHCP troubleshooting
* LAN troubleshooting
* VLAN configuration
* Cisco switch configuration
* Router configuration
* Connectivity testing
* Windows networking
* Linux networking
* Packet analysis
* Network documentation
* Incident troubleshooting
* Root-cause analysis
* Technical documentation

---

# 🎯 Career Relevance

These labs are designed to demonstrate practical skills relevant to roles such as:

* Network Support Engineer
* Technical Support Engineer
* IT Support Engineer
* IT Technician
* Service Desk Analyst
* Desktop Support Engineer
* NOC Engineer
* Network Administrator
* Infrastructure Support Engineer
* Cloud Support Engineer

The objective is not only to learn networking theory but also to practice a **real troubleshooting workflow** similar to what is used in IT support and network operations environments.

---

# 📈 Learning Approach

Each lab follows this cycle:

```text
Learn
  ↓
Build
  ↓
Break
  ↓
Troubleshoot
  ↓
Fix
  ↓
Verify
  ↓
Document
```

I intentionally practice both **normal configurations and broken configurations** so that I can develop troubleshooting skills rather than only following configuration tutorials.

---

# 📂 Repository Organization

Each scenario contains its own documentation and evidence:

```text
Scenario/
│
├── README.md
├── Ticket.md
│
└── Screenshots/
    ├── step-01.png
    ├── step-02.png
    ├── verification.png
    └── final-result.png
```

The `README.md` explains the technical procedure, while the ticket documentation records the issue, investigation, root cause, and resolution.

---

# ⚠️ Important Note

All screenshots, configurations, test results, and troubleshooting evidence added to this repository are based on my own hands-on lab work.

The purpose of this repository is to demonstrate practical networking knowledge through reproducible lab scenarios and documented troubleshooting.

---

# 👨‍💻 Author

**Manish Shinde**

M.Sc. Computer Science

**Areas of Focus:**

* IT Support
* Network Support
* System Administration
* Cloud Support
* IT Infrastructure

---

## ⭐ Repository Goal

> Build a practical networking portfolio that demonstrates the ability to **configure, troubleshoot, verify, and document real-world network support scenarios.**

