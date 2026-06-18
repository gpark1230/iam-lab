# Windows Server 2022 Deployment

## Business Requirement

Apex Innovations requires its first Windows Server to support the enterprise identity environment. This server will become DC01, the first Domain Controller for the organization.

## Implementation Status

In Progress

## Planned Configuration

| Setting | Value |
|---|---|
| VM Name | dc01 |
| Region | East US |
| Resource Group | rg-iam-lab-eastus-001 |
| Operating System | Windows Server 2022 Datacenter |
| Size | Standard B2s |
| Virtual Network | vnet-iam-lab-eastus-001 |
| Subnet | snet-servers-eastus-001 |
| Private IP | 10.10.1.10 |
| Public IP | Temporary for RDP |
| Disk Type | Standard SSD |

## Design Decision

The first Windows Server will be deployed in Azure to support Active Directory Domain Services, DNS, and future hybrid identity integration.

A cost-conscious VM size is used because this is a lab environment, while still providing enough resources for a functional Domain Controller.

## Validation

To be completed after deployment.

## Screenshots

To be added after deployment.

## References

- Microsoft Learn
- Azure Virtual Machines Documentation
- Active Directory Domain Services Documentation