# Kubernetes-Crash-Course


What is Kubernetes?
- Kubernetes aka (K8s) is a open source container orchestration system designed for automating the deployment, scaling, and management of containerized applications.
- TLDR - Kubernetes (K8s) is a container orchestrator. Companies will often deploy hundreds of containers and it's hard to manage all of them so admins will use K8s to manage all 100 of the containers.


# Key terms to know when learning about Kubernetes (K8s)
- Containers
- Nodes - a Kubernete node is a virtual machine that is part of a cluster.
- A node can be:
1. Virtual Machine (most common)
2. Physical server
3. Cloud VM
- Pod - pods hosts one or more containers. Pods are created and managed by K8s.

<img align="left" width="200" height="350" src="https://github.com/user-attachments/assets/c2cdb631-5768-416f-b8c3-c798409c4030">

- Containers in the same pod:
- - Share the same IP
- - Share storage
- - Share network namespace
- - Are scheduled together
- Image
- Docker
- Cluster - a "cluster" is a managed group of compute resources, specifically Azure Virtual Machines (VMs), that run containerized applications using Kubernetes orchestration.
- Kubectl - is the CLI for Kubernetes and it is how you manage Kubernetes Cluster.

Kubernetes and Container Architecture Visual
<img width="800" height="1380" alt="image" src="https://github.com/user-attachments/assets/75873797-9071-46d7-a6de-10d86132ee05" />

Kubernetes and Container Architecture Visual

<img width="400" height="636" alt="image" src="https://github.com/user-attachments/assets/36a04450-3c23-4e79-b964-49a251921add" />


# Real World Analogy

1. Node = Apartment Building
2. Pod = Single apartment
3. Container = Room inside the apartment
- You rent apartments (pods)
- Apartment live inside buildings (Nodes)
- Rooms (Containers) share walls, plumbing, and internet.



# What problem does Kubernestes solve?
- Problem: Managing containers at scale


# Key benefits: Automation, Scalability, High Availability


# How do you manager a AKS cluster?
- You manage AKS cluster via its API server. AKS clusters have a control plane API server that can be publicly accessible.



# Benefits of Kubernetes
- Self-healing for availability
- Scalability 


# Self Healing 
- What does self-healing mean when it's related to K8s?
- Example:
- 1. A pod crashes
- - If a container inside a pod crashes, kubelet will detect it and a pod is restarted automatically
- 2. A pod gets deleted
- - The ReplicaSet creates a new pod
- 3. Node failure
- - If a worker node goes down:
- - Pods on that node are rescheduled onto healthy nodes
 

# Scalability 
- Horizontal Pod Autoscaler (HPA)
- Scales from 1 -> Thousands of pods



# Azure Kubernetes vs Kubernetes
- AKS is Kubernetes operationalized and secured by Azure.

- Major AKS benefits
1. Managed control plane

Azure handles:
1. API server
2. etcd
3. Horizontal Availability
4. Patching
5. Upgrades
6. Certificates


