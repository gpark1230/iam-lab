# ADR-004: Administrative Account Strategy

## Status

Accepted

## Context

Privileged accounts present a high-value target for attackers.

## Decision

Every administrator receives:

- Standard user account
- Administrative account

Administrative accounts are only used for privileged operations.

---

## Rationale

Separating privileged identities reduces exposure to phishing, malware, and browser-based attacks.

---

## Consequences

### Benefits

- Supports Least Privilege
- Supports Zero Trust
- Reduces attack surface

### Tradeoffs

- Users manage two identities

---

## References

Microsoft Privileged Access Strategy