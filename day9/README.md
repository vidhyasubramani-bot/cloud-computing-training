# Kubernetes Website Deployment Using Minikube

## Project Overview

This project demonstrates how to deploy a Python web application on a local Kubernetes cluster using Minikube. The application is containerized with Docker and deployed as a Kubernetes Pod.

## Technologies Used

- Python
- Docker
- Kubernetes
- Minikube
- kubectl
- Ubuntu (AWS EC2)

## Project Workflow

1. Created a Python web application.
2. Created a Dockerfile for the application.
3. Built the Docker image.
4. Installed Docker, kubectl, and Minikube.
5. Started the Minikube cluster using Docker as the driver.
6. Created a Kubernetes Pod configuration (`pod.yml`).
7. Deployed the application using Kubernetes.
8. Verified the Pod status and inspected Pod details.

## Commands Used

### Install kubectl

```bash
curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"
chmod +x kubectl
sudo mv kubectl /usr/local/bin/
kubectl version --client
```

### Install Minikube

```bash
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
sudo install minikube-linux-amd64 /usr/local/bin/minikube
minikube version
```

### Start Minikube

```bash
minikube start --driver=docker --force
```

### Verify Cluster

```bash
kubectl cluster-info
kubectl get nodes
```

### Build Docker Image

```bash
docker build -t ubuntu-hospital-web .
```

### Deploy Pod

```bash
kubectl apply -f pod.yml
```

### Check Pod

```bash
kubectl get pods
kubectl describe pod hospital-pod
```

## Project Structure

```
hospital-project/
│── app.py
│── requirements.txt
│── Dockerfile
│── pod.yml
└── README.md
```

## Learning Outcomes

- Understood Kubernetes architecture.
- Learned how to install and configure kubectl and Minikube.
- Built Docker images for Python applications.
- Deployed a containerized application as a Kubernetes Pod.
- Verified and managed Pods using kubectl commands.
- Gained hands-on experience with local Kubernetes clusters.

## Conclusion

This project provided practical experience in deploying a containerized Python application using Kubernetes and Minikube. It improved my understanding of container orchestration, Pod management, and Kubernetes deployment workflows.
