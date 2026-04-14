# Martin Opedal

Lead Cloud Solution Architect at Microsoft. Azure Landing Zones, AKS, Terraform, security, sovereign cloud.

Ran datacenters for nearly a decade before this. Co-founded two craft breweries on the side. Most of what I ship here is built in collaboration with GitHub Copilot, including the agentic coding features. I do the architecture, Copilot handles the grunt work.

## Repos

Terraform modules, ARG queries, and tooling that came out of real customer engagements.

### Runners and CI/CD

| Repo | What it does | Stack |
|------|-------------|-------|
| [terraform-azurerm-avm-ptn-cicd-agents-and-runners](https://github.com/martinopedal/terraform-azurerm-avm-ptn-cicd-agents-and-runners) | Azure Verified Module for self-hosted ADO agents and GitHub runners. PAT and UAMI auth. | Terraform, Azure Container Apps |
| [terraform-azurerm-github-runners-alz-corp](https://github.com/martinopedal/terraform-azurerm-github-runners-alz-corp) | Self-hosted runners on Container Apps for ALZ Corp subscriptions. Central firewall egress, no public IPs. | Terraform, ACA, Azure Firewall |
| [ghec-vnet-runners-azure](https://github.com/martinopedal/ghec-vnet-runners-azure) | GitHub-hosted runners with Azure VNet integration. Built for GHE.com with EU data residency. | Terraform, Azure Networking |

### Landing Zones

| Repo | What it does | Stack |
|------|-------------|-------|
| [alz-graph-queries](https://github.com/martinopedal/alz-graph-queries) | 135 Azure Resource Graph queries for ALZ checklist validation. Takes automated coverage from 49 queries (19%) to 135 (53%). | PowerShell, ARG |

### Kubernetes

| Repo | What it does | Stack |
|------|-------------|-------|
| [terraform-azapi-aks-automatic](https://github.com/martinopedal/terraform-azapi-aks-automatic) | AKS Automatic with ALZ Corp networking. BYO VNet, multiple ingress options (AGC, NGINX, Istio), multiple egress options (NAT GW, UDR, LB). | Terraform, azapi |

### Operations

| Repo | What it does | Stack |
|------|-------------|-------|
| [azure-quota-reports](https://github.com/martinopedal/azure-quota-reports) | Collects compute and network quotas across Azure subscriptions. Exports to CSV. | PowerShell |

## Elsewhere

[LinkedIn](https://www.linkedin.com/in/martin-opedal). I write about Landing Zones, Kubernetes, and AI platforms there. I speak at NIC on Terraform, GitHub Copilot, and IaC security.
