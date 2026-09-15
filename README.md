# Mosh

## **Cloud and Platform Engineer**

### Azure · AWS · Terraform · Kubernetes

I build platforms other engineers deploy onto: governed from day one, secure by default, and documented well enough that the next person can change them safely.

Deep in Azure. Building out AWS. Currently working on a multi-cloud internal developer platform.

---

## Platform Work

### [stratum-platform](https://github.com/moshstaq/stratum-platform) — Multi-cloud internal developer platform _(in progress)_

A golden path onto either cloud, consuming the Azure and AWS landing zones below. Developers get a paved route to production without writing platform Terraform.

Phases 0–4 complete: platform foundations, cross-cloud module contracts, and a FastAPI application layer running on EKS ([stratum-workload](https://github.com/moshstaq/stratum-workloads)). Phases 5–6 — resilience, observability, production readiness — in progress.

The interesting problem is not deploying to two clouds. It is deciding where the abstraction should stop. Identity federation, IAM versus RBAC scoping and network primitives differ structurally between Azure and AWS; pretending otherwise produces Azure logic wearing AWS names.

### [taskflow-platform](https://github.com/moshstaq/taskflow-platform) — AKS workload platform

FastAPI services on AKS with Service Bus, deployed onto the Azure landing zone. Terraform, Helm, workload identity, no static credentials anywhere in the cluster or pipeline.

Its main design decision is a three-tier Terraform dependency model that resolves the circular dependency between managed identity creation and OIDC federated credential configuration — the identity needs the cluster's OIDC issuer, and the workload needs the identity. Splitting the apply into ordered tiers removes the manual bootstrap step most implementations leave in place.

### [azure-landing-zone](https://github.com/moshstaq/azure-landing-zone) — Azure platform foundation

Cloud Adoption Framework landing zone built in Terraform and deployed through GitHub Actions. Management group hierarchy, hub-spoke networking with Application Gateway ingress, Azure Policy governance, Private Endpoints, centralised Log Analytics, cost management.

Built to be consumed, not admired: `stratum-workload` and `taskflow-platform` both sit on top of it.

### [aws-landing-zone](https://github.com/moshstaq/aws-landing-zone) — AWS platform foundation

The AWS counterpart. Multi-account structure, IAM, networking and Terraform state handling, built to serve the same consumers as the Azure foundation without copying Azure's scoping model across.

### [azure-ado-delivery-pipeline](https://github.com/moshstaq/azure-ado-delivery-pipeline) — Delivery pipeline

Azure DevOps to Container Apps. Terraform, Trivy scanning in the pipeline, Key Vault, workload identity federation, build-once-and-promote across environments so the artefact that reaches production is the one that was tested.

---

## Stack

| Area                      | Tools                                                          |
| ------------------------- | -------------------------------------------------------------- |
| Cloud                     | Azure (primary), AWS                                           |
| Infrastructure as Code    | Terraform                                                      |
| Containers and Kubernetes | Docker, AKS, EKS, Helm, AGIC, CSI Secrets Store                |
| Identity and Security     | Entra ID, RBAC, OIDC, Managed Identities, Key Vault            |
| CI/CD                     | GitHub Actions, Azure DevOps                                   |
| Networking                | VNets, NSGs, Private Endpoints, Hub-Spoke, Application Gateway |
| Observability             | Log Analytics, KQL, Azure Monitor, CloudWatch                  |
| Scripting                 | Bash, Python, PowerShell                                       |

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

## Current Role

Senior Service Desk Engineer. I lead and mentor nine engineers across a 5,000+ device estate — hybrid identity, networking, Intune, M365. The platform work above is where I have taken that operational grounding and built the thing rather than supported it.

---

## Connect

Open to **Cloud Engineer**, **Platform Engineer** and **DevOps** Engineering roles UK, Hybrid or remote.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-moshstaq-blue?logo=linkedin)](https://linkedin.com/in/moshstaq)
[![Email](https://img.shields.io/badge/Email-Contact-red)](mailto:moshood.adisa@moshstaq.com)
