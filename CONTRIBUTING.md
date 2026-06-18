# Contributing

Thank you for your interest in contributing to the Enterprise IAM & Cloud Security Lab.

Although this repository is currently maintained by a single author, it follows engineering practices commonly used in enterprise environments.

---

# Engineering Standards

All contributions should:

- Follow Microsoft security best practices.
- Prioritize enterprise realism over lab simplicity.
- Include documentation for every major change.
- Validate all implementations before submission.
- Follow the Principle of Least Privilege.
- Align with Zero Trust security principles.

---

# Documentation Requirements

Every major implementation should include:

- Business Requirement
- Architecture Overview
- Design Decisions
- Implementation Steps
- Validation
- Screenshots
- Lessons Learned
- Interview Talking Points (when applicable)

---

# Code Standards

## PowerShell

- Follow approved PowerShell verb naming conventions.
- Include comment-based help where appropriate.
- Prefer reusable functions over duplicated code.
- Include basic error handling.

---

## Python

- Follow PEP 8 style guidelines.
- Include docstrings.
- Use meaningful variable names.
- Keep scripts modular and reusable.

---

# Pull Request Checklist

Before submitting a change:

- [ ] Documentation updated
- [ ] Screenshots added (if applicable)
- [ ] Validation completed
- [ ] Naming conventions followed
- [ ] No secrets or credentials committed
- [ ] Architecture documentation updated (if required)

---

# Branch Strategy

Feature work should be developed in feature branches before merging into `main`.

Example:

- feature/entra-connect
- feature/conditional-access
- feature/pim

---

# Commit Message Convention

Use concise, descriptive commit messages.

Examples:

- Deploy Windows Server domain controller
- Configure Active Directory organizational units
- Implement Microsoft Entra Connect
- Configure Conditional Access baseline
- Deploy Microsoft Sentinel