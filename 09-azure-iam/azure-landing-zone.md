# Azure Landing Zone

## Business Requirement

Apex Innovations requires a secure Azure foundation before deploying identity infrastructure workloads such as domain controllers, management servers, and future cloud security services.

## Implementation Status

In Progress

## Resources

| Resource Type | Name | Purpose |
|---|---|---|
| Resource Group | rg-iam-lab-eastus-001 | Logical container for Azure lab resources |
| Virtual Network | vnet-iam-lab-eastus-001 | Network boundary for Azure workloads |
| Subnet | snet-servers-eastus-001 | Server subnet for identity infrastructure |
| Network Security Group | nsg-servers-eastus-001 | Controls inbound and outbound traffic |

## Tags

| Tag | Value |
|---|---|
| Project | Enterprise-IAM-Lab |
| Environment | Lab |
| Owner | Gavin-Park |
| CostCenter | IAM-Lab |