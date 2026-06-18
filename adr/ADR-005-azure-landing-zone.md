# ADR-005: Azure Landing Zone Design

## Status

Accepted

## Context

Before deploying workloads, the organization requires a standardized Azure foundation.

## Decision

Create a dedicated landing zone containing:

- Resource Group
- Virtual Network
- Server Subnet
- Network Security Group

All future Azure resources will be deployed inside this landing zone.

---

## Rationale

Separating infrastructure from workloads improves organization, scalability, and security.

---

## Consequences

### Benefits

- Easier management
- Consistent networking
- Improved governance

### Tradeoffs

- Slightly more initial planning

---

## References

Microsoft Cloud Adoption Framework
Azure Well-Architected Framework