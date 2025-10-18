# AWS CI/CD Deployment Project

## Overview
This project demonstrates a simple **CI/CD pipeline** for deploying applications to **AWS EC2** using GitHub Actions and Terraform.  
It showcases automated builds, secure deployment, and infrastructure-as-code practices.

---

## Key Features
- **Automated CI/CD:** Code changes trigger builds and tests via GitHub Actions.  
- **Secure Deployment:** Artifacts are uploaded to EC2 instances via SSH/SCP.  
- **Infrastructure-as-Code:** Terraform manages Security Groups and deployment permissions.  
- **Dynamic Security:** GitHub Actions runner IPs are automatically allowed via Terraform.

---

## Tech Stack
- **CI/CD:** GitHub Actions  
- **Cloud:** AWS EC2  
- **IaC:** Terraform  
- **Scripting:** PowerShell / Bash  

---

## How It Works
1. Push code → triggers GitHub Actions workflow.  
2. Workflow builds, tests, and packages the app.  
3. Terraform updates EC2 Security Group rules for GitHub runners.  
4. Files are deployed to EC2 automatically.
5. The server restarts and new page is visible.  

---

```bash
git clone https://github.com/yourusername/aws-ci-cd.git
