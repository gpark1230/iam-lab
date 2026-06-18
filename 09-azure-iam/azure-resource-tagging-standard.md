# Azure Resource Tagging Standard

## Purpose

This document defines the mandatory Azure resource tagging standard used throughout the Enterprise IAM & Cloud Security Lab.

Resource tags improve governance, cost management, automation, inventory management, and operational visibility.

All Azure resources deployed within this project must follow this standard unless otherwise documented.

---

# Objectives

The Azure tagging strategy is designed to:

- Improve resource organization
- Support cost tracking
- Simplify administration
- Enable future automation
- Simulate enterprise cloud governance
- Align with Microsoft Azure best practices

---

# Required Tags

| Tag | Required | Description | Example |
|------|----------|-------------|---------|
| Project | Yes | Identifies the project owning the resource | Enterprise-IAM-Lab |
| Environment | Yes | Deployment environment | Lab |
| Owner | Yes | Primary resource owner | Gavin-Park |
| CostCenter | Yes | Cost allocation identifier | IAM-Lab |

---

# Current Tag Values

| Tag | Value |
|------|-------|
| Project | Enterprise-IAM-Lab |
| Environment | Lab |
| Owner | Gavin-Park |
| CostCenter | IAM-Lab |

---

# Future Tags

As the project grows, additional governance tags may be introduced.

| Tag | Purpose |
|------|----------|
| DataClassification | Public, Internal, Confidential, Restricted |
| Criticality | Low, Medium, High |
| Backup | Indicates whether backup policies apply |
| BusinessUnit | Department responsible for the workload |
| Application | Associated application or service |
| ManagedBy | Automation platform or administrator |
| Compliance | Regulatory requirements (PCI, HIPAA, etc.) |

---

# Design Decision

A standardized tagging strategy ensures every Azure resource can be identified, managed, and reported consistently.

Applying tags during resource creation supports governance from the beginning of the project rather than relying on retroactive tagging.

---

# Real-World Relevance

Enterprise organizations commonly enforce required tags using Azure Policy.

Mandatory tagging enables:

- Cost reporting
- Resource inventory
- Automation
- Security auditing
- Compliance reporting
- Operational ownership

Many organizations prevent Azure resources from being created if required tags are missing.

---

# Validation

When deploying Azure resources, verify that:

- All required tags are present.
- Tag names use consistent capitalization.
- Tag values match the enterprise standard.
- Resources appear correctly when filtered by tag in the Azure Portal.

---

# References

- Microsoft Learn – Organize Azure resources with tags
- Azure Well-Architected Framework
- Microsoft Cloud Adoption Framework