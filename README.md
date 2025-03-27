# SIT323 2025 Task 6.1P – Deploying a Containerized Node.js App to Kubernetes

## 📦 Overview

This project demonstrates how to deploy a containerized Node.js application to a local Kubernetes cluster using **Minikube**. The Node.js app was previously developed in Task 5.1P and has been reused, containerized with Docker, and successfully deployed and exposed via a Kubernetes Service.

## 🧰 Technologies Used

- Node.js
- Docker
- Docker CLI
- Kubernetes
- Minikube
- kubectl
- Git

## 🛠 What I Did

- Reused the Node.js application created in Task 5.1P (`server.js`)
- Created a Dockerfile to containerize the application
- Built the Docker image inside Minikube's Docker environment
- Wrote Kubernetes YAML files:
  - `deployment.yaml` – defines the Pod and container configuration
  - `service.yaml` – exposes the app via a NodePort service
- Used `kubectl` to deploy the application to the local Kubernetes cluster
- Verified that the Pod was running and Service was reachable
- Accessed the deployed app via a browser
- Documented the process and included screenshots

## 🚀 How to Run

> Make sure you have Docker Desktop, Minikube, and kubectl installed.

### 1. Start Minikube
```bash
minikube start --driver=docker
