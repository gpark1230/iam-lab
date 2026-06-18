# Enterprise Architecture

## Overview

The company operates a hybrid identity environment that integrates an on-premises Active Directory infrastructure with Microsoft Entra ID. Identity synchronization is handled by Microsoft Entra Connect, allowing users to access both on-premises and cloud resources using a single identity.

The environment follows Microsoft's Zero Trust security model by enforcing identity verification, least privilege access, and continuous monitoring.

---

# Physical Locations

## Headquarters
New York, NY

## Branch Office
Boston, MA

## Remote Workforce
Approximately 30% of employees work remotely.

---

# On-Premises Infrastructure

- Windows Server Domain Controller
- Active Directory Domain Services
- DNS
- DHCP
- File Server
- Group Policy
- Windows 11 Enterprise workstations

---

# Cloud Infrastructure

## Microsoft Azure

- Microsoft Entra ID
- Azure Virtual Machines
- Azure Storage
- Azure Key Vault
- Azure Monitor

## Microsoft 365

- Exchange Online
- Teams
- SharePoint Online
- OneDrive

## AWS

- IAM
- EC2
- S3

---

# Identity Flow

Users
↓

Active Directory

↓

Microsoft Entra Connect

↓

Microsoft Entra ID

↓

Microsoft 365
Azure
AWS
Enterprise Applications

---

# Security Stack

Identity

- Active Directory
- Microsoft Entra ID
- PIM
- Identity Governance

Endpoint Security

- Microsoft Defender

Monitoring

- Microsoft Sentinel

Authentication

- MFA
- Conditional Access
- SSO

Automation

- PowerShell
- Python

---

# Future Expansion

This environment is designed to support:

- Microsoft Intune
- Defender XDR
- Azure Landing Zones
- Terraform
- GitHub Actions
- SCIM provisioning
- Okta federation
- AWS Organizations