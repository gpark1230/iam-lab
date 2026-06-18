# Active Directory Design

## Table of Contents

1. Business Requirement
2. Domain Design
3. Organizational Unit Structure
4. Naming Conventions
5. Administrative Account Strategy

---

# 1. Business Requirement

Apex Innovations requires a centralized identity platform to manage employee authentication, authorization, workstation access, server access, and future integration with Microsoft Entra ID.

The Active Directory design must support secure administration, scalable user organization, Group Policy management, and future hybrid identity synchronization.

---

# 2. Domain Design

**Active Directory Domain**

```
corp.apexinnovations.com
```

**NetBIOS Name**

```
APEX
```

## Design Decision

The Active Directory forest will use the internal domain **corp.apexinnovations.com**.

Using a dedicated corporate subdomain separates internal identity infrastructure from public-facing services while aligning with Microsoft's modern Active Directory naming recommendations.

## Real-World Relevance

Modern enterprise environments typically avoid using **.local** for new Active Directory deployments. Instead, organizations commonly deploy Active Directory using a subdomain of a domain they own, simplifying DNS management and future hybrid identity integration with Microsoft Entra ID.

---

# 3. Organizational Unit Structure

## Proposed OU Design

```text
corp.apexinnovations.com
│
└── Apex
    │
    ├── Users
    │   ├── Executive
    │   ├── Human Resources
    │   ├── Finance
    │   ├── Information Technology
    │   ├── Security Operations
    │   ├── Software Engineering
    │   ├── Sales
    │   ├── Marketing
    │   ├── Customer Support
    │   ├── Contractors
    │   └── Vendors
    │
    ├── Groups
    │   ├── Security Groups
    │   ├── Distribution Groups
    │   └── Role-Based Access Groups
    │
    ├── Computers
    │   ├── Workstations
    │   ├── Laptops
    │   └── Shared Devices
    │
    ├── Servers
    │   ├── Domain Controllers
    │   ├── File Servers
    │   └── Application Servers
    │
    ├── Service Accounts
    ├── Admin Accounts
    └── Disabled Objects
```

## Design Decision

The Organizational Unit structure separates users, groups, computers, servers, service accounts, privileged accounts, and disabled objects into dedicated administrative boundaries.

Department-specific OUs support delegated administration, targeted Group Policy Objects (GPOs), and future growth without requiring structural redesign.

## Real-World Relevance

Enterprise Active Directory environments organize objects based on administration, security, and policy application rather than convenience. A well-designed OU hierarchy simplifies administration, auditing, delegation, and identity lifecycle management.

---

# 4. Naming Conventions

## User Accounts

| Account Type | Format | Example |
|--------------|--------|---------|
| Standard User | first.last | john.smith |
| Administrative User | adm-first.last | adm-john.smith |
| Contractor | ext-first.last | ext-jane.lee |
| Vendor | vnd-company-purpose | vnd-okta-support |
| Service Account | svc-application-purpose | svc-entra-sync |

---

## Computer Accounts

| Device Type | Format | Example |
|--------------|--------|---------|
| Workstation | WS-DEPT-001 | WS-FIN-001 |
| Laptop | LT-DEPT-001 | LT-IT-001 |
| Shared Device | SH-DEPT-001 | SH-HR-001 |

---

## Server Accounts

| Server Type | Format | Example |
|--------------|--------|---------|
| Domain Controller | DC01 | DC01 |
| File Server | FS01 | FS01 |
| Application Server | APP01 | APP01 |

---

## Security Groups

| Group Type | Format | Example |
|--------------|--------|---------|
| Security Group | SG-Resource-Permission | SG-Finance-Share-Read |
| Role Group | ROLE-Department-Function | ROLE-IT-Helpdesk |
| Distribution Group | DL-Department | DL-Finance |

## Design Decision

A standardized naming convention ensures identities, devices, groups, servers, and service accounts can be quickly identified throughout the environment.

Prefixes such as **adm-**, **svc-**, **ext-**, and **vnd-** clearly distinguish privileged, service, contractor, and vendor accounts.

## Real-World Relevance

Consistent naming standards improve operational efficiency, access reviews, troubleshooting, auditing, automation, and incident response while reducing administrative errors.

---

# 5. Administrative Account Strategy

## Principle of Least Privilege

All privileged administrators receive two separate identities.

### Standard User Account

Purpose

- Email
- Microsoft Teams
- Web browsing
- Microsoft 365
- Daily business activities

Example

```text
john.smith
```

---

### Administrative Account

Purpose

- Active Directory administration
- Domain Controller management
- Group Policy administration
- Azure administration
- PowerShell administration
- Server administration

Example

```text
adm-john.smith
```

Administrative accounts must never be used for routine business activities.

---

## Privileged Access Principles

- Separate standard and privileged identities
- Apply the Principle of Least Privilege
- Require Multi-Factor Authentication for privileged accounts
- Implement Microsoft Entra Privileged Identity Management (PIM)
- Audit privileged account activity
- Use Just-in-Time (JIT) privilege elevation where possible

## Real-World Relevance

Separating privileged identities from standard user accounts significantly reduces the risk of credential theft through phishing, malware, browser exploitation, or endpoint compromise.

This approach aligns with Microsoft's Zero Trust architecture and privileged access guidance.

## Future Enhancements

- Items that will be implemented in later phases of the project.

---

## References

- Microsoft Learn
- Microsoft Security Best Practices
- Microsoft Entra Documentation