# Azure Identity & Access Management (IAM) Lab

## 📌 Project Overview
This project demonstrates the setup of an enterprise-grade identity structure within Microsoft Entra ID (Azure AD). The goal was to move away from individual user management toward a scalable, group-based access model following the principle of **Least Privilege**.

## 🏗️ Phase 1: Identity Foundation (Manual Setup)

### 1. User Provisioning
I created a set of departmental users to simulate a real-world corporate environment:
* **Sarah Chen** (Finance)
* **Michael Ross** (IT)
* **James Doe** (HR)
* **Charles Sampson** (IT)
* **Frank Ford** (Finance)
* **Lilly Baxter** (HR)
    
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
<img width="951" height="757" alt="image" src="https://github.com/user-attachments/assets/a5296a9c-8055-41d0-a382-263958fc2be9" />


<img width="1352" height="587" alt="image" src="https://github.com/user-attachments/assets/038b8960-ec22-47ff-a7ed-8935179cb122" />


<img width="1345" height="702" alt="image" src="https://github.com/user-attachments/assets/6845789c-d896-4c1f-b57d-a62ed8a79ae9" />
