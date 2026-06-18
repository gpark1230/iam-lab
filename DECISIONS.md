# Architecture Decision Index

This document serves as the central index for all Architecture Decision Records (ADRs) within the Enterprise IAM & Cloud Security Lab.

Architecture Decision Records document significant technical and architectural decisions made throughout the project, including the rationale, alternatives considered, and long-term impact.

---

# Purpose

The purpose of maintaining ADRs is to:

- Record important architectural decisions.
- Explain the reasoning behind implementation choices.
- Improve long-term maintainability.
- Provide context for future project expansion.
- Demonstrate enterprise engineering documentation practices.

---

# Decision Status

| Status | Meaning |
|----------|---------|
| Proposed | Under discussion |
| Accepted | Approved and implemented |
| Superseded | Replaced by a newer decision |
| Deprecated | No longer recommended |

---

# Architecture Decision Records

| ADR | Title | Status |
|-----|-------|--------|
| ADR-001 | Hybrid Identity Strategy | Accepted |
| ADR-002 | Active Directory Domain Design | Accepted |
| ADR-003 | Organizational Unit Design | Accepted |
| ADR-004 | Administrative Account Strategy | Accepted |
| ADR-005 | Azure Landing Zone Design | Accepted |

---

# Future ADRs

The following Architecture Decision Records are expected to be added during future phases of the project.

## Identity

- ADR-006 Microsoft Entra Connect Synchronization Strategy
- ADR-007 Password Hash Synchronization vs Pass-through Authentication
- ADR-008 Conditional Access Baseline Policies
- ADR-009 Multi-Factor Authentication Strategy
- ADR-010 Role-Based Access Control Model
- ADR-011 Privileged Identity Management Design

---

## Cloud

- ADR-012 Azure Resource Organization
- ADR-013 Azure RBAC Strategy
- ADR-014 Azure Key Vault Design
- ADR-015 AWS IAM Design
- ADR-016 Cross-Cloud Identity Federation
- ADR-017 Okta Integration Strategy

---

## Security Operations

- ADR-018 Microsoft Sentinel Architecture
- ADR-019 Identity Logging Strategy
- ADR-020 Threat Detection Methodology
- ADR-021 Incident Response Workflow
- ADR-022 MITRE ATT&CK Mapping Strategy

---

## Automation

- ADR-023 PowerShell Automation Standards
- ADR-024 Microsoft Graph Automation
- ADR-025 Infrastructure as Code Strategy
- ADR-026 CI/CD Pipeline Design

---

# Engineering Principles

Every architectural decision in this project should:

- Support Zero Trust security principles.
- Follow the Principle of Least Privilege.
- Align with Microsoft best practices.
- Scale to enterprise environments.
- Prioritize automation where appropriate.
- Be fully documented.
- Include validation and testing.