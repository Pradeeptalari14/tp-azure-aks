# Azure AKS Cluster Studio

This repository contains the target configuration and SRE runtime files compiled by the **Azure AKS Cluster Studio** dashboard module.

## 🚀 Description
Orchestrate enterprise AKS clusters. Generate Terraform HCL, AKS network policies, azure-cni overlays, and Active Directory pod identity bindings.

## 🛠️ Specification Matrix
- **Primary Configuration File**: `/infra/aks/aks_cluster.tf`
- **Execution Command**: `terraform init && terraform apply -auto-approve`
- **Validation Command**: `terraform show`

## 📋 How to Run & Validate

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Pradeeptalari14/tp-azure-aks.git
   cd tp-azure-aks
   ```

2. **Run Execution Target:**
   ```bash
   terraform init && terraform apply -auto-approve
   ```

3. **Verify Runtime Stability:**
   ```bash
   terraform show
   ```

## 🔐 Security & Best Practices
* **Secret Isolation**: Use organization-level secrets (or SSM parameter hooks) rather than hardcoded environment variables inside files.
* **Pull Request Lifecycles**: Protect default branch merges with validation checks before merging code changes.
