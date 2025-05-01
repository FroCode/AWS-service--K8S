# 🌍 Advanced DevOps Project

This repository demonstrates a complete CI/CD pipeline using **Terraform**, **Jenkins**, **Kubernetes (EKS)**, and **ArgoCD**, enabling automated deployment of a Node.js application on AWS infrastructure.

---

## 📐 Architecture Diagram

![devops-task](https://github.com/AbdelrhmanAli123/advanced-devops-task/assets/133269614/3948183e-9730-411a-b9a3-0b0ebc302fc3)

---

## ⚙️ Tech Stack

- **Infrastructure as Code**: Terraform  
- **Containers**: Docker  
- **Orchestration**: Kubernetes (EKS)  
- **CI/CD**: Jenkins, ArgoCD, Helm  
- **Database**: Amazon RDS  
- **Networking**: NGINX Ingress, Cert-Manager, Route53  
- **IAM Integration**: OIDC/IRSA  
- **App**: Node.js + Express

---

## 📝 Prerequisites

- AWS CLI and credentials configured  
- Terraform, Helm, Kubectl, Docker installed  
- A registered domain with a hosted zone in Route53  
- Jenkins with access to GitHub and AWS  

---

## 📊 App Overview

A Node.js API with two endpoints:

- `/client-ip` – stores client IP in RDS  
- `/client-ip/list` – returns all stored IPs

---

## 📁 Project Structure

```bash
.
├── terraform/                 # IaC to provision EKS, RDS, VPC, etc.
├── k8s/                       # Kubernetes manifests (Deployment, Service, Secrets)
├── helm/                      # Helm chart for the app
├── jenkins_files/            # CI/CD pipeline scripts
├── app/                       # Node.js source code
└── README.md                  # You're here
