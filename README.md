# Mosh A

**Cloud and Platform Engineer** | Azure | Terraform | Kubernetes

---

On-prem taught me what breaks. Cloud taught me how to scale.
I build infrastructure that is secure by default, governed from day one, and simple enough for the next engineer to understand.

---

## What I Have Built

### [Azure Landing Zone](https://github.com/moshstaq/azure-landing-zone)

A production-pattern Azure platform built from scratch using Terraform and GitHub Actions, implementing Cloud Adoption Framework landing zone patterns. Not a template. Not a wizard. Every resource is defined in code, every deployment runs through CI/CD.

Covers the full platform stack management group hierarchy, hub-spoke networking with Application Gateway ingress, Azure Policy governance, AKS with workload identity, Private Endpoints, centralised observability, disaster recovery and cost management.

### [Azure AKS Platform Onboarding](https://github.com/moshstaq/azure-aks-platform-onboarding)

End-to-end workload onboarding onto the landing zone above. Python FastAPI application containerised with a multi-stage Dockerfile, pushed to Azure Container Registry, deployed to AKS via Helm, with secrets fetched from Key Vault using workload identity no credentials stored anywhere in the cluster or pipeline.

GitHub Actions CI/CD pipeline builds, scans with Trivy, and deploys on every push to main. All managed identity values are read dynamically from Azure CLI at runtime so the pipeline survives infrastructure reprovisioning without manual intervention. Every deployment step is idempotent safe to run multiple times against the same cluster.

---

## Stack

| Area                      | Tools                                                          |
| ------------------------- | -------------------------------------------------------------- |
| Cloud                     | Azure (primary)                                                |
| Infrastructure as Code    | Terraform                                                      |
| Containers and Kubernetes | Docker, AKS, Helm, AGIC, CSI Secrets Store                     |
| Identity and Security     | Entra ID, RBAC, OIDC, Managed Identities, Key Vault            |
| CI/CD                     | GitHub Actions, Azure DevOps                                   |
| Networking                | VNets, NSGs, Private Endpoints, Hub-Spoke, Application Gateway |
| Observability             | Log Analytics, KQL, Azure Monitor                              |
| Scripting                 | Bash, PowerShell, Python                                       |

---

## Certifications

| Certification                            | Issuer    |
| ---------------------------------------- | --------- |
| AZ-104 Microsoft Azure Administrator     | Microsoft |
| SC-300 Identity and Access Administrator | Microsoft |
| MD-102 Endpoint Administrator            | Microsoft |
| AZ-900 Azure Fundamentals                | Microsoft |
| CC Certified in Cybersecurity            | ISC²      |

---

## How I Work

I understand before I deploy.
I prevent rather than fix.
I master fundamentals over trends — stacks change, engineers who understand why things work will always adapt.

---

## Connect

Open to **Cloud Engineer**, **Platform Engineer** and **DevOps** roles across the UK and the rest of the world. Hybrid and remote.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-moshstaq-blue?logo=linkedin)](https://linkedin.com/in/moshstaq)
[![Email](https://img.shields.io/badge/Email-Contact-red)](mailto:moshood.adisa01@gmail.com)

📍 England
