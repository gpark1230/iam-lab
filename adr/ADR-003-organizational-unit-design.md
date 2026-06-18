# ADR-003: Organizational Unit Design

## Status

Accepted

## Context

The enterprise requires a scalable method of organizing users, computers, servers, and administrative objects.

## Decision

Organize Active Directory using department-based Organizational Units with separate containers for:

- Users
- Computers
- Servers
- Groups
- Service Accounts
- Administrative Accounts

---

## Rationale

This design supports delegated administration, Group Policy targeting, auditing, and future organizational growth.

---

## Consequences

### Benefits

- Easier administration
- Better Group Policy management
- Clear security boundaries

### Tradeoffs

- Slightly more planning required during deployment

---

## References

Microsoft Active Directory Best Practices