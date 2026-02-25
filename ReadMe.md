# TerraformFoundry: Automated Infrastructure as a Product (IaP)

*Inspired by Hephaestus — the god who built the tools of the gods.*

## 1. Overview
**TerraformFoundry** is a curated, professionally maintained library of production-grade Terraform modules designed to provision complete, secure, and compliant cloud environments on **Oracle Cloud Infrastructure (OCI)**. It is specifically engineered for the East African tech sector, with built-in compliance for **Bank of Uganda** and **NITA-U** standards.

## 2. The Problem
Infrastructure fragility in emerging markets is often a result of "click-ops" and undocumented manual configurations. This leads to **Brain Drain Risk**, where critical knowledge leaves when an engineer departs, and **Compliance Gaps**, where systems are not auditable or reproducible.

## 3. The Solution
TerraformFoundry transforms infrastructure from a manual service into a **codified product**.
-   **Resilience through Reproducibility:** Rebuild your entire environment from zero in under 20 minutes.
-   **Auditability by Default:** 100% of resource changes are logged and tagged.
-   **Security as Code:** Least-privilege IAM policies and data-at-rest encryption are baked into every module.

## 4. Platform Modules
1.  **Networking Foundation:** VCN, Public/Private Subnets, NAT, and Internet Gateways.
2.  **Managed Kubernetes (OKE):** Automated cluster provisioning, autoscaling, and ingress control.
3.  **Managed PostgreSQL:** Secure, private-placement database with automated backups.
4.  **Observability Stack:** Prometheus and Grafana for full-stack monitoring and alerting.
5.  **Identity & Access (IAM):** Role-based access control and environment isolation.
6.  **CI/CD Pipeline:** GitHub Actions-driven "Plan-and-Apply" workflow.

## 5. Quick Start
To deploy the entire stack from zero, ensure you have the [OCI CLI](https://docs.oracle.com/en-us/iaas/Content/API/SDKDocs/cliinstall.htm) and [Terraform](https://developer.hashicorp.com/terraform/downloads) installed.

```bash
# Clone the repository
git clone https://github.com/cloudarchitects-africa/terraformfoundry.git
cd terraformfoundry

# Initialize Terraform
terraform init

# Plan your infrastructure (review the changes)
terraform plan -var-file="environments/prod.tfvars"

# Apply and watch the environment materialize
terraform apply -var-file="environments/prod.tfvars" -auto-approve
```

## 6. Project Documentation
Detailed deep-dive documentation is available in the `docs/` folder:
-   [01 Executive Overview](./docs/01-Executive/Project%20Proposal%20Report.md)
-   [02 System Architecture](./docs/02-Architecture/System_Architecture.md)
-   [03 System Design](./docs/03-System-Design/System_Design.md)
-   [04 Module Details](./docs/04-Modules/)
-   [06 Security & Compliance](./docs/06-Security/Security_Compliance.md)
-   [10 Project Roadmap](./docs/10-Roadmap/Project_Roadmap.md)

## 7. Business Model
TerraformFoundry is the engine behind **CloudArchitects Africa**. We offer:
-   **Foundation Packages:** One-time production-ready IaC setup.
-   **Module Subscriptions:** Continuous updates to our module library.
-   **Compliance-as-a-Product:** Pre-configured environments for BoU and NITA-U audits.

## 8. License
Copyright © 2026 CloudArchitects Africa. All rights reserved.
For commercial licensing inquiries, contact [licensing@cloudarchitects.africa](mailto:licensing@cloudarchitects.africa).
