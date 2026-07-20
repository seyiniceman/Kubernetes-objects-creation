# Kubernetes Objects Creation

Deploy and manage core Kubernetes resources using YAML manifests to demonstrate Kubernetes administration, application deployment, networking, configuration management, and Role-Based Access Control (RBAC).

---

## Project Overview

This project demonstrates the creation and management of fundamental Kubernetes objects using declarative YAML manifests.

The repository contains examples of commonly used Kubernetes resources including Deployments, Services, Namespaces, ConfigMaps, Service Accounts, Cluster Role Bindings, and the Kubernetes Dashboard. These manifests demonstrate how applications are deployed, configured, secured, and exposed within a Kubernetes cluster.

This project showcases practical Kubernetes administration skills and follows declarative Infrastructure as Code principles for managing containerized workloads.

---

## Architecture Diagram

```text
                     +----------------------+
                     |      Developer       |
                     +----------+-----------+
                                |
                                | kubectl apply -f
                                v
                     +----------------------+
                     |   Kubernetes API     |
                     +----------+-----------+
                                |
      +------------+------------+------------+------------+
      |            |            |            |            |
      v            v            v            v            v
 Deployment   Service    ConfigMap    Namespace    ServiceAccount
      |                                             |
      |                                             |
      +----------------+----------------------------+
                       |
                       v
              ClusterRoleBinding
                       |
                       v
             Kubernetes Dashboard
                       |
                       v
              Running Kubernetes Cluster
```

---

## Objectives

- Deploy applications using Kubernetes Deployments.
- Expose applications using Services.
- Configure applications using ConfigMaps.
- Organize workloads with Namespaces.
- Implement Kubernetes RBAC.
- Deploy and access the Kubernetes Dashboard.
- Demonstrate declarative Kubernetes resource management.

---

## Technologies Used

- Kubernetes
- YAML
- kubectl
- Docker
- Linux
- Git

---

## Repository Structure

- deployment.yaml
- service.yaml
- namespace.yaml
- configmap.yaml
- configmap-pod-1.yaml
- configmap-pod-2.yaml
- clusterrole-binding.yaml
- sa.yaml
- kubernetes-dashboard.yaml
- README.md

---

## Workflow

1. Create a Kubernetes namespace.
2. Deploy the application using a Deployment manifest.
3. Create a Service to expose the application.
4. Configure application settings using ConfigMaps.
5. Create a Service Account.
6. Configure Cluster Role Binding for permissions.
7. Deploy the Kubernetes Dashboard.
8. Verify all resources using kubectl.

---

## Prerequisites

- Kubernetes Cluster
- kubectl installed
- Docker
- Linux environment
- Git

---

## Deployment Steps

1. Clone the repository.

```bash
git clone <repository-url>
```

2. Create the namespace.

```bash
kubectl apply -f namespace.yaml
```

3. Deploy the application.

```bash
kubectl apply -f deployment.yaml
```

4. Create the service.

```bash
kubectl apply -f service.yaml
```

5. Apply the ConfigMap.

```bash
kubectl apply -f configmap.yaml
```

6. Create the Service Account.

```bash
kubectl apply -f sa.yaml
```

7. Create the Cluster Role Binding.

```bash
kubectl apply -f clusterrole-binding.yaml
```

8. Deploy the Kubernetes Dashboard.

```bash
kubectl apply -f kubernetes-dashboard.yaml
```

9. Verify resources.

```bash
kubectl get all
kubectl get pods
kubectl get svc
kubectl get configmaps
kubectl get namespaces
```

---

## Skills Demonstrated

- Kubernetes Administration
- Kubernetes Deployments
- Services
- Namespaces
- ConfigMaps
- Service Accounts
- RBAC
- Kubernetes Dashboard
- YAML
- kubectl
- Linux
- Git

---

## Project Outcome

Successfully created and managed essential Kubernetes resources using declarative YAML manifests. The project demonstrates practical Kubernetes administration, including application deployment, service exposure, configuration management, namespace isolation, Role-Based Access Control (RBAC), and cluster management through the Kubernetes Dashboard. It showcases best practices for managing Kubernetes workloads using Infrastructure as Code principles.

# Author

**Seyi Akinmusere**

DevOps | Cloud Engineer | AWS | Terraform | Jenkins | Docker | Kubernetes

