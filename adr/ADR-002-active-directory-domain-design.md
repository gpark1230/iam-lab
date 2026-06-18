# ADR-002: Active Directory Domain Design

## Status

Accepted

## Context

The organization requires an internal Active Directory namespace.

## Decision

Use:

corp.apexinnovations.com

NetBIOS:

APEX

---

## Rationale

Using a subdomain of the corporate domain follows Microsoft's current recommendations and simplifies future Microsoft Entra integration.

---

## Consequences

### Benefits

- Modern Microsoft best practice
- Simplified DNS
- Cleaner hybrid identity

### Tradeoffs

- Requires ownership of the public domain name

---

## References

Microsoft Learn