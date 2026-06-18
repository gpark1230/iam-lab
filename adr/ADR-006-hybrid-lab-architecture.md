# ADR-006: Hybrid Lab Architecture

## Status

Accepted

## Context

The original design proposed hosting Windows Server in Azure.

Azure Free Trial subscriptions have compute quota limitations that prevent deployment of the required virtual machines without upgrading to a Pay-As-You-Go subscription.

Rather than introducing unnecessary cost, the project will adopt a hybrid architecture.

## Decision

The enterprise Active Directory infrastructure will be hosted on a dedicated Windows desktop running local virtualization.

Microsoft Azure will host cloud identity services including:

- Microsoft Entra ID
- Conditional Access
- Privileged Identity Management
- RBAC
- Log Analytics
- Microsoft Sentinel

The on-premises Active Directory environment will synchronize identities to Microsoft Entra ID using Microsoft Entra Connect.

## Consequences

Advantages

- Eliminates Azure VM costs
- Allows multiple virtual machines
- Better reflects many enterprise environments
- Supports richer Active Directory scenarios

Disadvantages

- Requires a dedicated lab workstation
- Infrastructure is split between local virtualization and Azure