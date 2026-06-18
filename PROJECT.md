# Enterprise IAM & Cloud Security Lab

## Project Overview

This repository documents the design, implementation, and operation of a fictional enterprise Identity & Access Management (IAM) environment for Apex Innovations.

The objective is to simulate the work of an IAM Engineer, Cloud Security Engineer, or Security Engineer by designing and implementing a modern hybrid identity infrastructure using Microsoft technologies, AWS, and industry security best practices.

This project follows a real engineering lifecycle: **Design → Build → Secure → Monitor → Automate**.

---

# Project Status

## Current Phase

🟡 Phase 2 — Infrastructure Deployment

## Current Sprint

🚧 Sprint 2 — Azure Foundation & Domain Controller Deployment

---

# Completed Milestones

## Sprint 1 — Enterprise Design ✅

- [x] Initialize Git repository
- [x] Connect repository to GitHub
- [x] Create repository structure
- [x] Create project README
- [x] Design company profile
- [x] Design enterprise architecture
- [x] Design enterprise network
- [x] Design Active Directory architecture
- [x] Design Organizational Unit structure
- [x] Design enterprise naming conventions
- [x] Design privileged account strategy

---

# Sprint 2 — Azure Foundation & Domain Controller Deployment

## BR-001 — Establish Azure Landing Zone

**Status**

COMPLETE!!!

### Tasks

- [x] Create Resource Group
- [x] Apply resource tags
- [x] Create Virtual Network
- [x] Create Server subnet
- [x] Configure Network Security Group
- [x] Validate networking

---

## BR-002 — Deploy Windows Server 2022

**Status**

⬜ Not Started

### Tasks

- [ ] Deploy Windows Server 2022 VM
- [ ] Configure static private IP
- [ ] Configure storage
- [ ] Review NSG rules
- [ ] Connect using Remote Desktop
- [ ] Validate server deployment

---

## BR-003 — Install Active Directory Domain Services

**Status**

⬜ Not Started

### Tasks

- [ ] Install AD DS role
- [ ] Promote DC01 to Domain Controller
- [ ] Create forest
- [ ] Configure DNS
- [ ] Validate AD installation

---

## BR-004 — Build Enterprise Active Directory

**Status**

⬜ Not Started

### Tasks

- [ ] Create Organizational Units
- [ ] Create Security Groups
- [ ] Create Administrative Accounts
- [ ] Create Service Accounts
- [ ] Create Standard User Accounts
- [ ] Validate authentication

---

# Upcoming Phases

## Phase 3 — Hybrid Identity

- Microsoft Entra ID
- Microsoft Entra Connect
- Hybrid Identity Synchronization
- Password Hash Synchronization
- Seamless SSO

---

## Phase 4 — Identity Security

- Conditional Access
- Multi-Factor Authentication
- Role-Based Access Control (RBAC)
- Identity Governance
- Access Reviews
- Entitlement Management

---

## Phase 5 — Privileged Access

- Microsoft Entra Privileged Identity Management (PIM)
- Just-in-Time Administration
- Administrative Units
- Privileged Access Groups

---

## Phase 6 — Cloud Identity

### Microsoft Azure

- Azure RBAC
- Managed Identities
- Azure Key Vault
- Azure Storage
- Azure Virtual Machines

### AWS

- IAM Users
- IAM Groups
- IAM Roles
- Cross-Account Access
- Identity Federation

### Okta

- Enterprise SSO
- SCIM Provisioning
- Identity Federation

---

## Phase 7 — Security Operations

- Microsoft Sentinel
- Identity Monitoring
- KQL Analytics Rules
- Incident Response
- Threat Hunting
- MITRE ATT&CK Mapping

---

## Phase 8 — Automation

- PowerShell
- Microsoft Graph API
- Azure PowerShell
- Python
- Automated User Provisioning
- Automated Offboarding

---

# Repository Structure

```text
enterprise-iam-security-lab/
│
├── 01-enterprise-architecture/
├── 02-active-directory-services/
├── 03-hybrid-identity/
├── 04-entra-id/
├── 05-conditional-access/
├── 06-rbac/
├── 07-identity-governance/
├── 08-pim/
├── 09-azure-iam/
├── 10-aws-iam/
├── 11-okta-sso/
├── 12-sentinel-detection/
├── 13-incident-response/
├── scripts/
├── diagrams/
├── docs/
├── PROJECT.md
└── README.md
```

---

# Engineering Principles

- Build for enterprise realism rather than certification objectives.
- Follow Microsoft's Zero Trust architecture.
- Apply the Principle of Least Privilege.
- Automate repetitive administrative tasks whenever possible.
- Document every design decision.
- Validate every implementation.
- Design for scalability.
- Treat every change as if it were made in a production enterprise.

---

# Long-Term Roadmap

Future enhancements include:

- Microsoft Defender XDR
- Microsoft Intune
- Microsoft Purview
- Microsoft Entra Verified ID
- Azure Landing Zones
- Terraform
- GitHub Actions
- Infrastructure as Code
- Multi-forest Active Directory
- Enterprise PKI
- Active Directory Certificate Services
- High Availability Domain Controllers

---

# Last Updated

June 2026