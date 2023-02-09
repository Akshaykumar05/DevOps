# Welcome to DevOps Guide 
![DevOps](../assets/DevOps.webp)
## What is DevOps?

DevOps is a movement and a culture before being a job this is why cultural aspects are very important. DevOps is all about getting your solutions to run efficiently from deployment to updates.
The two groups, operations and development are converged into a single group where the engineers work across the whole SDLC(Software Development Life Cycle).
The development team that develops the plan, designs and builds the system from scratch and the operation team for testing and implementation of whatever is developed. The operations team gave the development team feedback on any bugs that needed fixing and any rework required. Invariably, the development team would be idle awaiting feedback from the operations team. This undoubtedly extended timelines and delayed the entire software development cycle. There would be instances where the development team moves on to the next project while the operations team continues to provide feedback for the previous code. This meant weeks or even months for the project to be closed and final code to be developed. Now, what if the two departments came together and worked in collaboration with each other?

## To become a DevOps Engineer, you need to know about:
* Linux
* Networking
* Version Control System
* Cloud Service: AWS/Azure/GCP
* Python/Bash
* Docker
* Kubernetes
* CI/CD

## Linux

## Networking

## Version Control System
So when you work in teams, most likely there will be some kind of version control system. It could be github, bit-bucket or gitlab. So they all work with git, which is why you need to have an understanding of it. With my personal experience, I had to learn how branching worked, how you create a pull request and what kind of git workflow the team followed. So understanding the basics of git is necessary.

### What is a Version Control System?
Version control is the ability to understand the various changes that happened to the code over time (and possibly roll back). All these are enabled by using a version control system such as Git. A Git repository can live on one’s machine, but it usually lives on a central online or on-prem repository. Benefits are:

* Collaborate with other developers
* Make sure the code is backed-up somewhere
* Make sure it’s fully viewable and auditable

You might ask why Git? Git is a de facto standard. Git is the most broadly adopted tool of its kind. Vast numbers of developers already have Git experience and a significant proportion of college graduates may have experience with Git.

## Resource:

| Resource                                                            | Notes                                                                                       |
| :------------------------------------------------------------------ | :----------------------------------------------------------------------------------------- |
| [Kunal Kushwaha - Complete Git and GitHub Tutorial](https://youtu.be/apGV9Kg7ics)|  This tutorial will help you with using Git & GitHub for your personal projects.
| [Apoorv Goyal - Git and GitHub Materclass](https://youtu.be/LQ2LTPHeTts)| This  tutorial will focuses on Introduction to Git for  absolute beginners with no prior coding experience.

## Kubernetes
* Kubernetes is an open-source **Container Management tool** which automates container deployment, container scaling and load balancing.
* It schedules, runs and manage isolated containers which are running on virtual/physical/ cloud support.
* All top cloud providers support Kubernetes.

### History of K8s
* Google developed an internal system called 'borg' (later named Omega) to deploy and manage thousands google applications and their services on cluster.
* In 2014, Google introduced Kubernetes an Open source Plateform written in 'Golang'  and later donated to CNCF.

### Online Plateform for K8s
* Kubernetes playground
* Play with K8s
* Play with Kubernetes Classroom

### Cloud Based K8s Services
* GKE- Google Kubernetes Services
* AKS- Azure Kubernetes Services
* Amazon EKS- Elastic Kubernetes Services

### Kubernetes Instalation Tool
* Minicube
* Kubeadm

### Problems with Scaling up the Containers
* Containers can not communicate with each other.
* Autoscaling and Load Balancing was not possible.
* Containers had to be managed carefully.

### Features of K8s
* Orchestration (Clustering of any no of containers running on different network)
* Autoscaling (Vertical & Horizontal)
* Auto-Healing
* Load Balancing
* Plateform Independent (Cloud/Virtual/Physical)
* Fault Tolerance (Node/PoD failure.
* Rollback (going back to previous version)
* Health Monitoring of Containers.
* Batch Execution (one time sequential, Parallel)

| Features                                   |Kubernetes                                             | Docker Swarm                                                                                       
| :------------------------------------------| :-----------------------------------------------------| :--------------------------------------------------------- |
| Installation and Cluster Configuration | Complicated and time consuming | Fast and Easy
| Supports | K8s can work with almost all container types like Rocket, Docker, Container | 
| GUI | GUI Available | GUI not available
| Data Volumes | Only shared with Containers in same Pod | can be shared with any other container
| Updates and Rollback | Process scheduling to maintain services while updating | Progressive updates and service health monitoring throughout the update
| Autoscaling | Support vertical and horizontal Autoscaling | Not support Autoscaling
| Logging and Monitoring | Inbuild tool present for monitoring | used 3rd party tools like splunk

### Working with K8s:
* We create manifest (.yml)
* Apply this to cluster (to master) to bring into desired state.
* Pod runs on node, which is controlled by master.

### Role of Master Node
Kubernetes cluster contains Containers running or Bare Metal/ VM instances/ Cloud instances/ all mix.
* K8s designates one or more of these as master and other as workers.
* The master is now going to run set of K8s processes. These processes will ensure  smooth functioning of Cluster, these process are called "Control Plane"
* Can be multi-master for high availability
* Master runs Control Plane to run cluster smoothly

### Components of Control Plane (Master)
1. Kube-api-server
2. etcd
3. Kube-Scheduler
4. Controller Manager

#### 1 Kube-api-server
* The api-server interacts directly with user (i.e. we apply .yml pr json manifest to Kube-api-server)
* This Kube-api-server is meant to scale automatically as per load.
* Kube api-server is fron-end of Control-plane.

#### 2 etcd
* Stores metadata (data of data) and status of cluster.
* etcd is Consistent and high-available store (key-value store)
* Source of touch for cluster state (info about state of cluster)

#### etcd has following features:
1. **Fully Replicated**- The entire state is available on every node in the cluster.
2. **Secure**- Implements aitomatic TLS with optional Client-Certificate authentication.
3. **Fast**- Benchmarked at 10,000 writes per second

