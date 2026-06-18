# Network Design

## Network Overview

The enterprise operates a single headquarters with one branch office and remote employees.

The primary Active Directory infrastructure resides at headquarters.

---

# Headquarters Network

Network

192.168.10.0/24

Gateway

192.168.10.1

---

# Servers

| Server | IP Address |
|----------|------------|
| Domain Controller | 192.168.10.10 |
| File Server | 192.168.10.20 |
| Management Server | 192.168.10.30 |

---

# Client Devices

DHCP Range

192.168.10.100 - 192.168.10.200

---

# DNS

Primary DNS

192.168.10.10

---

# Future Azure Resources

Azure Virtual Network

10.10.0.0/16

Subnet

10.10.1.0/24

VPN Gateway

Future Implementation

---

# Future AWS Resources

VPC

172.16.0.0/16

Public Subnet

172.16.1.0/24

Private Subnet

172.16.2.0/24

---

# Remote Access

Remote employees authenticate through Microsoft Entra ID using Conditional Access policies and Multi-Factor Authentication.

Administrative access requires Privileged Identity Management and Just-in-Time elevation.

---

# Security Principles

- Least Privilege
- Zero Trust
- Role-Based Access Control
- MFA Everywhere
- Administrative Separation
- Centralized Logging