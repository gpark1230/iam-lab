# ADR-001: Hybrid Identity Strategy

## Status

Accepted

---

## Date

June 2026

---

## Context

Apex Innovations requires a centralized identity platform that supports both traditional Active Directory workloads and modern cloud services such as Microsoft 365, Microsoft Entra ID, Azure, and AWS.

The architecture must provide a migration path from on-premises identity to cloud identity while minimizing disruption to users and existing infrastructure.

---

## Decision

The organization will adopt a **Hybrid Identity** architecture using:

- Active Directory Domain Services (AD DS)
- Microsoft Entra ID
- Microsoft Entra Connect

Active Directory will remain the authoritative source for user identities while Microsoft Entra ID provides cloud authentication and access to Microsoft 365 and Azure resources.

---

## Rationale

A hybrid identity model provides:

- Centralized identity management
- Single Sign-On (SSO)
- Compatibility with legacy applications
- Modern cloud authentication
- Simplified migration to cloud services

---

## Consequences

### Benefits

- Supports gradual cloud adoption
- Enables centralized identity management
- Integrates with Microsoft 365
- Supports Conditional Access
- Supports MFA
- Supports Identity Governance

### Tradeoffs

- Additional synchronization infrastructure
- More complex identity troubleshooting
- Increased operational complexity

---

## References

- Microsoft Learn
- Microsoft Entra Hybrid Identity Documentation