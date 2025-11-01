
# Azure Kubernetes Service (AKS) Deployment Project

## 📋 Project Overview
A complete cloud-native application deployment on Azure Kubernetes Service demonstrating container orchestration, CI/CD practices, and infrastructure automation.

## 🏗️ Architecture
[Client] → [Azure Load Balancer] → [AKS Cluster] → [Node.js Microservices]
↓
[Azure Container Registry]

text

## 🚀 Features Deployed
- **Containerized Node.js Application** with health endpoints
- **AKS Cluster** with auto-scaling node pool
- **Azure Load Balancer** with public IP exposure
- **Health Monitoring** with liveness/readiness probes
- **Horizontal Pod Distribution** across cluster nodes

## 📊 Deployment Status
- **Pods**: 2/2 Running ✅
- **Services**: LoadBalancer Active ✅  
--**External Access**: Load Balancer Configured ✅
- **Container Registry**: Integrated ✅

## 🛠️ Technology Stack
- **Kubernetes**: Azure AKS
- **Container Runtime**: Docker
- **Registry**: Azure Container Registry (ACR)
- **Networking**: Azure Load Balancer
- **Application**: Node.js + Express.js
- **Monitoring**: Kubernetes Dashboard & Azure Monitor

## 📁 Project Structure
aks-azure-lab/
├── src/ # Application source code
├── kubernetes/ # K8s manifests
├── docker/ # Docker configuration
├── docs/ # Documentation
└── README.md

text

## 🔧 Quick Start
```bash
# Deploy to AKS
kubectl apply -f kubernetes/deployment.yaml
kubectl apply -f kubernetes/service.yaml

# Verify deployment
kubectl get all
📈 Monitoring & Logs
bash
# Check pod status
kubectl get pods -w

# View application logs
kubectl logs -f deployment/aks-demo-app

# Monitor service
kubectl get service aks-demo-app-service
🙏 Acknowledgments
This hands-on learning experience was made possible through the cloud infrastructure and educational platform provided by Al Nafi. The practical exposure to enterprise-grade container orchestration on Azure has been invaluable for professional growth in cloud-native technologies.

Developer: Raees Malik
Contact: raees.malik89@gmail.com
GitHub: raeesmalik89-oss

Successfully deployed and tested on Azure Kubernetes Service
