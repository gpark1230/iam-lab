# Security Policy

## Purpose

This repository documents a fictional enterprise Identity & Access Management (IAM) environment for educational and portfolio purposes.

It is not intended for production use.

---

# Responsible Disclosure

If you discover a security issue within this repository, please report it through GitHub Issues.

Do not publish sensitive information, credentials, or exploit details.

---

# Repository Security

The following items must never be committed:

- Passwords
- API Keys
- Azure Secrets
- Client Secrets
- Certificates
- Private Keys
- Access Tokens
- Connection Strings
- Production Credentials

---

# Secret Management

Sensitive values should be stored using:

- Azure Key Vault
- Environment Variables
- Secure Secret Stores

Never store secrets directly in source code.

---

# Lab Environment

This project uses isolated lab environments only.

No production systems are connected to this repository.

Any company names, users, domains, and infrastructure are fictional unless otherwise noted.

---

# Security Principles

The project follows:

- Zero Trust
- Principle of Least Privilege
- Defense in Depth
- Secure by Default
- Identity First Security

---

# Compliance

Where applicable, design decisions align with guidance from:

- Microsoft Learn
- Microsoft Security Best Practices
- Microsoft Cloud Adoption Framework
- Azure Well-Architected Framework
- CIS Benchmarks