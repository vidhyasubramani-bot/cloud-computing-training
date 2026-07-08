🚀 Deploying a Three-Tier Architecture Application on AWS EKS using GitHub Actions, Argo CD, Prometheus, and Grafana

📌 Project Overview

This project demonstrates the deployment of a Three-Tier Architecture Application on Amazon EKS (Elastic Kubernetes Service) using modern DevOps practices. It implements CI/CD automation, GitOps deployment, and real-time monitoring to provide a scalable, reliable, and production-ready application deployment workflow.

---

🏗 Project Architecture

The application follows a Three-Tier Architecture consisting of:

- Presentation Layer (Frontend) – Provides the user interface.
- Application Layer (Backend) – Processes business logic and API requests.
- Database Layer – Stores application data.

Deployment and monitoring are automated using DevOps tools such as GitHub Actions, Argo CD, Prometheus, and Grafana.

---

🛠 Technologies Used

- AWS
- Amazon EKS
- Kubernetes
- Docker
- Git & GitHub
- GitHub Actions
- Argo CD
- Prometheus
- Grafana
- Python Flask
- MySQL

---

📂 Project Workflow

1. Developer writes application code.
2. Code is pushed to GitHub.
3. GitHub Actions automatically builds the Docker image.
4. Docker image is pushed to Docker Hub.
5. Argo CD detects changes in the Git repository.
6. Argo CD deploys the latest manifests to the Amazon EKS cluster.
7. Kubernetes manages Pods, Deployments, and Services.
8. Prometheus collects application and cluster metrics.
9. Grafana displays monitoring dashboards.

---

⚙️ Prerequisites

Before starting, install the following:

- AWS CLI
- Docker
- kubectl
- eksctl
- Terraform
- Git
- Helm
- Jenkins (optional)
- Argo CD CLI (optional)

Create:

- AWS Account
- GitHub Account
- Docker Hub Account

---

🚀 Deployment Steps

Step 1: Create AWS Infrastructure

- Configure AWS CLI
- Create VPC
- Create Amazon EKS Cluster
- Configure kubectl

---

Step 2: Build Docker Image

- Create Dockerfile
- Build Docker Image
- Push Image to Docker Hub

---

Step 3: Deploy to Kubernetes

Create Kubernetes manifests for:

- Namespace
- Deployment
- Service
- ConfigMap
- Secret
- Persistent Volume
- Persistent Volume Claim

Deploy using kubectl.

---

Step 4: Configure GitHub Actions

Create a GitHub Actions workflow to:

- Build Docker Image
- Push Docker Image
- Update Kubernetes manifests

---

Step 5: Configure Argo CD

- Install Argo CD
- Connect Git Repository
- Create Application
- Enable Auto Sync

---

Step 6: Install Prometheus

Deploy Prometheus to monitor:

- CPU Usage
- Memory Usage
- Pod Status
- Node Metrics
- Cluster Health

---

Step 7: Install Grafana

Connect Grafana with Prometheus.

Create dashboards for:

- CPU Utilization
- Memory Usage
- Pod Monitoring
- Network Traffic
- Cluster Performance

---

📊 Monitoring

Prometheus continuously collects metrics from the Kubernetes cluster.

Grafana visualizes these metrics using interactive dashboards to monitor application health and performance.

---

📸 Project Screenshots

The project documentation includes screenshots of:

- AWS Console
- EKS Cluster
- Kubernetes Nodes
- Pods
- Services
- GitHub Repository
- GitHub Actions Pipeline
- Docker Hub Repository
- Argo CD Dashboard
- Prometheus Dashboard
- Grafana Dashboard
- Running Application

---

📖 Documentation

A detailed project document is included containing:

- Introduction
- Project Architecture
- Prerequisites
- Installation
- Infrastructure Setup
- Deployment Steps
- CI/CD Pipeline
- GitOps Workflow
- Monitoring Setup
- Screenshots
- Results
- Conclusion

---

🎯 Learning Outcomes

After completing this project, you will understand:

- Cloud Computing
- AWS Services
- Amazon EKS
- Kubernetes
- Docker Containerization
- CI/CD using GitHub Actions
- GitOps using Argo CD
- Monitoring using Prometheus
- Visualization using Grafana
- End-to-End DevOps Workflow

---

🌟 Features

- Three-Tier Architecture
- Automated CI/CD Pipeline
- GitOps-Based Deployment
- Kubernetes Orchestration
- Containerized Application
- Automated Scaling
- Self-Healing Infrastructure
- Real-Time Monitoring
- Interactive Dashboards
- High Availability

---

📌 Conclusion

This project demonstrates how modern DevOps tools can automate application deployment, management, and monitoring on AWS. By integrating Amazon EKS, Docker, GitHub Actions, Argo CD, Prometheus, and Grafana, the deployment process becomes faster, more reliable, scalable, and easier to maintain.

---



Vidhya S

BE Computer Science and Engineering

Nehru Institute of Technology

Coimbatore, Tamil Nadu
