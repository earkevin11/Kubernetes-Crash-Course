# Kubernetes-Crash-Course


What is Kubernetes?
- Kubernetes aka (K8s) is a open source container orchestration system designed for automating the deployment, scalaing, and management of containerized applications.
- TLDR - Kubernetes (K8s) is a container orchestrator. Companies will often deploy hundreds of containers and it's hard to manage all of them so admins will use K8s to manage all 100 of the containers.

Key terms to know when learning about Kubernetes (K8s)
- Containers
- Nodes - a Kubernete note is a virtual machine that is part of a cluster.
- Pod - pods hosts one or more containers. Pods are created and managed by K8s.
- Image
- Docker
- Cluster - a "cluster" is a managed group of compute resources, specifically Azure Virtual Machines (VMs), that run containerized applications using Kubernetes orchestration.
- Kubectl - is the CLI for Kubernetes and it is how you manage Kubernetes Cluster. 


What problem does Kubernestes solve?
- Problem: Managing containers at scale


Key benefits: Automation, Scalability, High Availability


How do you manager a AKS cluster?
- You manage AKS cluster via its API server. AKS clusters have a control plane API server that can be publicly accessible.
