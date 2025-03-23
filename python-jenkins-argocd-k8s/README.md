

# Python-Jenkins-ArgoCD-K8s: Orchestrating CI/CD on Kubernetes

# 🍁 Introduction
Welcome to the Python-Jenkins-ArgoCD-K8s project! This repository provides a hands-on approach to implementing a modern CI/CD pipeline using Python, Jenkins, and ArgoCD on a Kubernetes cluster. By following this guide, you'll see practical insights into deploying robust and scalable applications with efficient automation and deployment strategies.


[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
        [![LinkedIn](https://img.shields.io/badge/LinkedIn-Profile-blue)](https://www.linkedin.com/in/nikhil--chaudhari/)
        [![Medium](https://img.shields.io/badge/Medium-Writeups-black)](https://medium.com/@nikhil-c)    




 

# 🍁 Pre-requisites
#### 1. System Requirements:
- Minimum 8 GB RAM and 4 CPU cores.
- Docker installed and running.
- Git installed.
#### 2. Tools Required:
- Python (version 3.8 or higher).
- **Jenkins:** Downloaded or containerized version.
- **Minikube:** A local Kubernetes cluster.
- **ArgoCD** installed and configured.

# 🍁Setup
Follow these steps to set up the project:
#### 1. Clone the Repository:
```bash
git clone https://github.com/DNcrypter/Jenkins-Kubernetes-Projects.git
cd Jenkins-Kubernetes-Projects/python-jenkins-argocd-k8s
```
#### 2. Set Up Jenkins:
- Install Jenkins as a Docker container or on your local machine.
- Configure Jenkins pipelines for **`CI/CD`**.

#### 3. Prepare Kubernetes Cluster:
- Deploy **`Minikube`** on your local machine.
- Install Kubernetes CLI tools like **`kubectl`**.

#### 4. Deploy ArgoCD:
- Install **`ArgoCD`** to your local Kubernetes cluster.
- Connect **`ArgoCD`** with your Jenkins setup.

#### 5. Build and Deploy:
- Use Jenkins pipelines to containerize the Python application.
-  Configure **`ArgoCD`** to sync deployments to Kubernetes.

#### 6. Run and Test:
- Validate the deployment using Kubernetes commands:
```bash
kubectl get pods
kubectl get services
```





# django-todo
A simple todo app built with django

![todo App](img_1)

## CICD Architecture [GitHub -> Jenkins -> k8s Manifests -> Argo CD -> k8s cluster]

![img 2](img_2)







# 🍁 Conclusion
By following the steps outlined here, we have created a fully functional CI/CD pipeline and shown, how to do application orchestration, deployment, and containerization using **`kubernetes`**.


### Thanks for checking out this project! Happy automation! 🚀










