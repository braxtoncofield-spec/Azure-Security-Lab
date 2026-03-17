# Azure Identity & Access Management (IAM) Lab

## 📌 Project Overview
This project demonstrates the setup of an enterprise-grade identity structure within Microsoft Entra ID (Azure AD). The goal was to move away from individual user management toward a scalable, group-based access model following the principle of **Least Privilege**.

## 🏗️ Phase 1: Identity Foundation (Manual Setup)

### 1. User Provisioning
I created a set of departmental users to simulate a real-world corporate environment:
* **Sarah Chen** (Finance)
* **Marcus Ross** (IT Admin)
* **John Doe** (HR)

### 2. Group-Based Access Control (GBAC)
Instead of assigning permissions to individuals, I created Security Groups:
* `GRP-Finance-Staff`
* `GRP-IT-Staff`
* `GRP-HR-Staff`

### 3. Role-Based Access Control (RBAC) Implementation
I restricted the **IT Group** to a specific scope to prevent "Privilege Creep":
* **Scope:** Resource Group `RG-Project-Alpha`
* **Role:** Contributor
* **Logic:** Members of IT can manage all resources within this project but cannot delete the subscription or modify global security settings.

---
## 📸 Evidence & Screenshots
