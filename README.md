# Martin

I build Azure platforms for regulated Nordic enterprises. Mostly Landing Zones, AKS, Terraform, private networking, and the parts that break when the diagram meets production.

Cloud Solution Architect, based in Oslo. Started with Azure in 2011 at a Norwegian systems integrator, ran datacenters through that decade, and now architect Landing Zones, AKS Automatic, and AI Foundry deployments for banks, government, energy, and defense customers in the Nordics.

I write longer-form on [opedal.tech](https://opedal.tech). Shorter posts on Landing Zones, AKS, and IaC security on [LinkedIn](https://www.linkedin.com/in/martin-opedal).

## Highlights

- Contributor to an Azure Verified Modules pattern proposal: [`terraform-azurerm-avm-ptn-cicd-agents-and-runners`](https://github.com/martinopedal/terraform-azurerm-avm-ptn-cicd-agents-and-runners) (not yet upstream)
- 135 Azure Resource Graph queries for the ALZ checklist, lifting automated coverage from the baseline 49 to 135
- NIC speaker on Terraform, GitHub Copilot, and IaC security. Live-streamed Level 300 session, 94% approval
- Microsoft Certified Azure Solutions Architect Expert, Cybersecurity Architect Expert, DevOps Engineer Expert
- Repos here come from regulated customer constraints: private endpoints, central firewall egress, ALZ Corp networking, sovereign and air-gapped setups

## Speaking

| Venue | Session | Signal |
|---|---|---|
| Nordic Infrastructure Conference (NIC) | Live-streamed Level 300 session on Terraform, GitHub Copilot, IaC security | 94% approval |
| Internal conference events | Architecture and platform sessions | 50 to 100 in-person, 200+ virtual |

Open to speaking on Azure Landing Zones, AKS Automatic, Terraform and AVM, IaC security, and AI-assisted infrastructure development. Reach me via [opedal.tech](https://opedal.tech).

## Repos

Same grouping I use on [opedal.tech](https://opedal.tech), with a few extras that have not made it onto the site yet.

### Azure governance and assessment

| Repo | What it does | Stack |
|------|--------------|-------|
| [azure-analyzer](https://github.com/martinopedal/azure-analyzer) | Bundled assessment runner that unifies azqr, PSRule, AzGovViz, and 135 ALZ Graph queries into one portable JSON and HTML report. | PowerShell |
| [alz-graph-queries](https://github.com/martinopedal/alz-graph-queries) | 135 Azure Resource Graph queries for the 255-item ALZ checklist. Takes automated coverage from the baseline 49 queries to 135. | PowerShell, ARG |
| [alz-checklist-queries](https://github.com/martinopedal/alz-checklist-queries) | ALZ checklist validation package built around the same 135 Azure Resource Graph checks for Landing Zone assessment. | PowerShell, ARG |
| [mcp-server-azure-architect](https://github.com/martinopedal/mcp-server-azure-architect) | Read-only MCP server and Copilot CLI skills bundle for Azure architects. Complements the official azure-mcp with ALZ checklist queries by ID and scorecard composition. | Python, MCP |
| [agentic-alz](https://github.com/martinopedal/agentic-alz) | Multi-stage GitOps orchestrator for ALZ Accelerator, AVM, and Terraform with narrow LLM stages for interview, design, drift triage, and firewall change composition. LLMs draft, humans approve, CI applies. | Python, LangGraph, OPA |
| [FinOps-assessment](https://github.com/martinopedal/FinOps-assessment) | Read-only audit of licensing and cost across Microsoft 365, Entra, Defender, Purview, Power Platform, Azure, GitHub, and Azure DevOps. Emits right-sizing and saving recommendations. Never mutates. | Python |

### AI Foundry and private AI platforms

| Repo | What it does | Stack |
|------|--------------|-------|
| [terraform-azurerm-avm-ptn-aifoundry-citadel](https://github.com/martinopedal/terraform-azurerm-avm-ptn-aifoundry-citadel) | Citadel pattern for private Azure AI Foundry with APIM and Azure Container Apps in an AVM-aligned landing zone. | Terraform, AzAPI, AVM |
| [terraform-azurerm-avm-ptn-aifoundry-citadel-gateway](https://github.com/martinopedal/terraform-azurerm-avm-ptn-aifoundry-citadel-gateway) | Terraform port of the Citadel governance gateway layer for private AI hub ingress and policy boundaries. | Terraform, APIM, AI Foundry |

### GitHub runners and CI/CD

| Repo | What it does | Stack |
|------|--------------|-------|
| [terraform-azurerm-avm-ptn-cicd-agents-and-runners](https://github.com/martinopedal/terraform-azurerm-avm-ptn-cicd-agents-and-runners) | AVM-style pattern module proposal for self-hosted ADO agents and GitHub runners with PAT and UAMI auth. No public IP egress. Not yet upstream in Azure Verified Modules. | Terraform, Azure Container Apps |
| [terraform-azurerm-github-runners-alz-corp](https://github.com/martinopedal/terraform-azurerm-github-runners-alz-corp) | Self-hosted GitHub Actions runners that run inside ALZ Corp landing zones with central firewall egress. | Terraform, ACA, Azure Firewall |
| [github-runners-alz-corp-cookbook](https://github.com/martinopedal/github-runners-alz-corp-cookbook) | Patterns, recipes, and drop-in workflows for the ALZ Corp self-hosted runner module. | Terraform, GitHub Actions |
| [terraform-azurerm-vmss-github-runners-windows](https://github.com/martinopedal/terraform-azurerm-vmss-github-runners-windows) | Windows VMSS GitHub Actions runner module wrapping the AVM virtual machine scale set module. | Terraform, VMSS |
| [terraform-azurerm-avm-ptn-cicd-agents-and-runners-personal](https://github.com/martinopedal/terraform-azurerm-avm-ptn-cicd-agents-and-runners-personal) | Public personal-runner lineage for testing the AVM-style CI/CD agents and runners pattern outside the upstream proposal. | Terraform, Azure Container Apps |
| [ghec-vnet-runners-azure](https://github.com/martinopedal/ghec-vnet-runners-azure) | GitHub-hosted runners with Azure VNet integration for GHE.com. EU data residency, private endpoint connectivity. | Terraform, Azure Networking |

### Kubernetes

| Repo | What it does | Stack |
|------|--------------|-------|
| [terraform-azapi-aks-automatic](https://github.com/martinopedal/terraform-azapi-aks-automatic) | AKS Automatic with ALZ Corp networking. BYO VNet, multiple ingress (AGC, NGINX, Istio), multiple egress (NAT GW, UDR, LB). | Terraform, azapi |
| [aks-automatic-ingress-migration](https://github.com/martinopedal/aks-automatic-ingress-migration) | Migration runbook and IaC for moving AKS Automatic ingress to Application Gateway for Containers. Bicep and Terraform parity, Gateway API. | Terraform, Bicep, AGC |

### Tooling

| Repo | What it does | Stack |
|------|--------------|-------|
| [azure-quota-reports](https://github.com/martinopedal/azure-quota-reports) | Collects compute and network quotas across Azure subscriptions. Exports to CSV. | PowerShell |
| [obsidian-memory-template](https://github.com/martinopedal/obsidian-memory-template) | Obsidian-based persistent memory system for GitHub Copilot. Karpathy pattern with Squad agents. | Markdown, Templater |
| [linkedin-auto-poster](https://github.com/martinopedal/linkedin-auto-poster) | RSS to LinkedIn pipeline. Ingests tech feeds, scores relevance, researches claims, drafts in your voice, ships through a GitHub PR approval workflow. | Python, GitHub Actions |

## Other repos

The list below regenerates from public repos via [`.github/workflows/update-readme.yml`](.github/workflows/update-readme.yml). Anything new on my GitHub appears here until I curate it into a section above. Repos with no description or no push in 12 months are filtered out so this section stays signal, not inventory.

<!-- repos:more:start -->
<!-- generated by scripts/update-readme.ps1, do not edit by hand -->

_No additional public repos to surface right now. Every active repo with a description is curated above._
<!-- repos:more:end -->

## Closing

The architecture, constraints, and review are mine. On the side I co-founded two craft breweries in Norway (Cervisiam, Krecher). Fermentation and infrastructure both reward tight feedback loops.

If something here helped, a star or a follow is appreciated. It helps more than people think when I submit to CFPs, and issues or PRs are always welcome.

Find me elsewhere: [opedal.tech](https://opedal.tech), [LinkedIn](https://www.linkedin.com/in/martin-opedal).
