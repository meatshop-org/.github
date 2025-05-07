# CI/CD Pipelines – Jenkins | AWS EC2 | Kubernetes | GitOps

Welcome to the official GitHub organization for the **CI/CD Automation Project**.  
This organization contains two repositories:

- **Frontend**: React js-based application  
- **Backend**: Django-based REST API  

Both are integrated into a Jenkins-powered CI/CD system with security, testing, and deployment pipelines.

## 🔧 What This Project Does

This CI/CD project is designed to:
- Automate testing, code analysis, and vulnerability scanning
- Build Docker images and push to DockerHub
- Deploy code to two different environments based on Git workflow:
  - **Feature branches** → deployed to **AWS EC2**
  - **Pull request branches** → deployed to **Kubernetes** via **GitOps** (ArgoCD)



---

## 🧩 Architecture

The architecture below illustrates the full CI/CD workflow — from GitHub commits to automated deployments across two environments: **AWS EC2** and **Kubernetes via ArgoCD**.

![CI/CD Pipeline Architecture](https://github.com/user-attachments/assets/451398a4-e13f-485d-b508-d5835b00d018)

## 📦 Key Features

- **Jenkins Pipelines** for both frontend and backend
- **Static Analysis (SAST)** with SonarQube
- **Dependency & Container Scanning** with npm audit, pip-audit, Trivy, OWASP Dependency Check
- **Dynamic Analysis (DAST)** using OWASP ZAP
- **Test Automation** for backend with unit tests + coverage
- **GitOps Workflow**: Kubernetes deployments via manifest repo and PR automation
- **Artifact Storage** on AWS S3 (reports, coverage, vulnerability scans)

## 📂 Repositories

| Repository | Description |
|------------|-------------|
| [`frontend`](https://github.com/BRHM1/frontend) | React-based frontend application with its own Jenkinsfile |
| [`backend`](https://github.com/BRHM1/backend) | Django backend with full test coverage and CI/CD integration |

## 📌 Note

This organization is built specifically to demonstrate a full-stack CI/CD pipeline with **dual deployment targets** and **secure DevOps practices**.  
It's an educational and practical project showcasing automated delivery pipelines in real-world environments.

---

Feel free to explore the repos and review the Jenkinsfiles to understand the complete flow from commit to deployment.
