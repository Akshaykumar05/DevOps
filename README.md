# Welcome to DevOps Guide 
![](https://assets-global.website-files.com/622642781cd7e96ac1f66807/62d0f091fc73b7a5828854b1_022021-Harness-Blogpost-DevOpsGeneric-Header-2400x700-1.png)

## What is DevOps?

DevOps is a movement and a culture before being a job this is why cultural aspects are very important. DevOps is all about getting your solutions to run efficiently from deployment to updates.
The two groups, operations and development are converged into a single group where the engineers work across the whole SDLC(Software Development Life Cycle).
The development team that develops the plan, designs and builds the system from scratch and the operation team for testing and implementation of whatever is developed. The operations team gave the development team feedback on any bugs that needed fixing and any rework required. Invariably, the development team would be idle awaiting feedback from the operations team. This undoubtedly extended timelines and delayed the entire software development cycle. There would be instances where the development team moves on to the next project while the operations team continues to provide feedback for the previous code. This meant weeks or even months for the project to be closed and final code to be developed. Now, what if the two departments came together and worked in collaboration with each other?

## To become a DevOps Engineer, you need to know about:
* Linux
* Networking
* Version Control System (Git and GitHub)
* Cloud Service: AWS/Azure/GCP (start with any one cloud provider)
* Infrastructure as a Code (IaaC) 
* Rrogramming language- Python/Bash
* Container- Docker
* Container Orchestration- Kubernetes
* CI/CD Pipeline
* Infrastructure provisioning- (Tool- Terraform)
* Configuration Management.(Tool- Ansible/Chef/Puppet)
* Microservices & 3-Tier structure
  
## Linux
### Some Important Commands:
* whoami - To check current user
* touchfile_name.txt - create file
* pwd - to check current workng directory
* mkdir foldername - to create a directory (folder)
* ls - to list content in current directory
* cd dirname - to change directory
* cd.. - to move one directory back
* mv src_path destination_path
* cat filename - to view contents of file.
* clear - to clear terminal.
* echo "your text" - to print something.
* ls -la -list contents of directory with file details.
* nano file_name -to write something in a file 
(To exit nano: ctrl+ × > press y if want to save or press n for no > press enter)
* history -to see all your previously executed commands
 rm filename -to delete the file
* cd -to go home directory

## Important topics to cover in Networking (Basics)
1. OSI Model (7 layers)
2. How system communicate.
3. LAN/WAN
4. What is switch, router, ISP(Internate Service Provider)
5. IP Address and types 
6. Basic Subnetting
7. DNS Basics (important)
8. Switching and routing

###  Linux Bash and Networking fundamentals
* For more in detail [Learn to Cloud](https://learntocloud.guide/docs/phase1/)
* [OSI Model and its 7 layers](https://www.imperva.com/learn/application-security/osi-model/)

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

## Cloud Service: AWS/Azure/GCP (start with any one cloud provider)
* For cloud I have done Microsoft Azure Fundamentals (az-900) certificate.
* I have written a blog about how I did free with all resorces, you can [read](https://akshaykumar05.hashnode.dev/microsoft-azure-fundamentals-az-900-exam) the blog here.
* You can also visit my [Cloud Computing Repo](https://github.com/Akshaykumar05/Cloud-Computing) where I have documented some cloud related stuff.
  
### Microservices
![](https://raw.githubusercontent.com/paulc4/microservices-demo/master/shopping-system.jpg)
## Docker
### Advantages of Docker
* No pre-allocation of RAM.
* CI efficiency- Docker enables you to build a container image and use that same image across every steps of the deployment process.
* Less cost.
* It is light in weight.
* It can run on physical h/w and virtual h/w or on Cloud.
* You can re-use the image.
* It took very less time to create container.

### Disadvantages of Docker
* Docker is not a good solution which requires a rich GUI (Graphics User Inerface)
* Difficult to manage large amount of container.
* Docker does not provide cross-platform compatibility means if an application is designed to run in a docker container on windows, then it can't run on Linux or vice-versa.
* Docker is suitable when the development OS and the testing OS are same.
* No solution for data recovery and back up.

### Docker Components
[](https://res.cloudinary.com/practicaldev/image/fetch/s--Jne8jX-C--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/aojpt8fs65jv79iqg4g2.png)
#### Docker Daemen
* Docker Daemen runs on the host O.S.
* It is responsible for running container to manage Docker services.
* Docker Daemon can communicate with other Daemon.

#### Docker Client
* Docker user can interact with Docker Daemen through a client (CLI)
* Docker client uses commant and rest API to communicate with the Docker Daemen.
* When a client run any server command on the Docker client 'terminal' the client terminal send these Docker commands to the docker daemen.
* It is possible for docker client to communicate more then one daemen.

### Docker Hub/Registry
* Docker registry manages and stored the docker images.
* There are two types of registries in docker
1. Public Registry- this is also called as docker hub.
2. Private Registry- It is used to share the images within the enterprices.

### Docker Images
* Docker images are th read only binary templates used to create docker Containers.
* Or it is a single file with all the dependencies and configuration required to run a programe or Container.
**Ways to create an image**
1. Take image from docker hub.
2. Create image from docker file.
3. Create image from existing docker containers.

### Docker Container
* Container holds the entire packages that is need to run an application.
* Or in other words we can say that the image is a template and a container is a copy of that template.
* Container is like a virtual machine.
* Images becomes container when they run on docker engine.

### Docker Image creation
* Docker images are templates used to create docker containers.
* Container is a running instance of image.

### Docker Commands
### Dockerfile:
* It is a text file with instructions to build image **automation of Docker image creation**.
### Some interview questions related to Docker
1. What are Images?
* Docker images are templates used to ctreate Docker containers.
2. Where are images stored.
* Registries(e.i. docker hub)
* Can be stored locally or remotely.
3. Other points.
* Docker can build images automatically by reading the instructions from a Dockerfile.
* Containers are running instances of Docker images.
* A single image can be used to create multiple containers.

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

#### 3 Kube-scheduler (action)
* When users make request for the creation and management of Pods, Kube-scheduler is going to take action on these request.
* Handle Pod creation and Management.
* Kube-scheduler match/assign any node to create and run pods.
* A scheduler watches for newly created Pods that have no node assigned for every pod that the scheduler discovers, the scheduler becomes responsible for finding best node for that pod to run on.
* Scheduler gets the information for hardware configuration from configuration files and the Pods on nodes accordingly

#### 4 Controller-Manager
Make sure actual state of cluster matches to desired state.

Two possible choices of Controller Manager
1. If K8s on cloud, then it will be Cloud-Controller-Manager.
2. If k8s on non-cloud, then it will be Kube-Controller-Manager.

#### Components on master that runs Containainer
1. **Node-Controller**- For checking the cloud provider to determine if a node has been detected in the Cloud after it stops responding.
2. **Server Controller**- Responsible for load Balancers on your cloud against services of typse Load Balancer.
3. **Volume Controller**- For creating, attaching and mounting volumes and interacting with the cloud provider to orchestrate volume.

#### Nodes (Kubelet and Container Engine)
Node is going to run 3 important piece of software/process.

1. **Kubelet**
* Agent running on the node
* Listens to Kubernetes master (eg- pod creation request)
* Use Port 10255
* Send success/fail reports to master

2. **Container Engine** (Docker)
* Works with Kubelet.
* Pulling images.
* Start/stop Containers.
* Exposing containers on ports specified in manifest.

3. **Kube-proxy**
* Assign IP to each Pod.
* It is required to assign IP address to pods (dynamic)
* Kube-proxy runs on each node and this make sure that each pod will get its own unique IP address.

These 3 coponents collectively consist "node"

### POD
* Smallest unit in Kubernetes
* Pod is a group of one or more containers that are deployed together on the same host. 
* A cluster is a group of nodes.
* A cluster has atleast one worker node and master node.
* In Kubernetes, the control unit is the POD, not containers.
* Consist of one or more tightly coupled containers
* Pod runs on node, which is controled by master.
* Kubernetes only knows about PODs ( does not know about individual container)
* Can not start containers without a POD.
* One POD usually contains one container.

#### Multi-Container PODS
* Share access to memory space.
* Connect to each other using localhost (Container port)
* Share access to the same volume.
* Containers within pod are deployed in an all-or-nothing manner.
* Entire pod is hosted on the same node (Scheduler will decide about which node)

#### POD Limitations
* No auto-healing or auto scaling.
* Pod crashes

#### Higher level K8s Objects
* Replication set- auto scaling and auto healing
* Deployment- Versioning and Rollback
* Service- Static (Non-epheneral) IP and Networking
* Volume- Non-epheneral storage 

#### Important
* Kubectl- Single Storage
* Kubeadm- On premise
* Kubefed- Federated

## CI/CD
* CICD is Continuous Integration and Continuous Deployment.
* CICD is a method to frequently deliver apps to customer by introducing Automation into the stages of app development.
* App development includes the stages like Test, Build and Deploy, which can be automated by CICD pipeline.
* Using CICD code from developer laptop to the production can be tested and deployed as it is pushed in repository like GitHub and Gitlab.
* This makes deployment faster and  with better quality.
* Tools used for this process are: **Jenkins, Gitlab, circleci**

### JENKINS
* Jenkins is an Open-Source project written in **Java** that runs on windows, MacOS and other Unix-Lite Operating systems. It is free, Community supported and might be your frst choice tool for CI.
* Jenkins automate the entire Software Development Life Cycle (SDLC)
* Jenkins was originally developed by Sun Microsystem in 2004 under the name of hudson.
* The project was later named jenkins when Oracle bought Microsystems.
* It can run on any major plateform without any compatibility issues.
* Whenever developer write Code, we integrate all that Code of all developers at that point of time and we build, test and deliever/deploy to the client. This prrocess is called CI/CD
* Jenkins helps us to achieve this.
* Because of CI, New bugs will be reported fast and get retified fast. So The entire software development happens fast.

#### Workflow of Jenkins
* We can attach Git, Maven, Selenium and Artifactory plugins to Jenkins.
* Once developers puts code in GitHub, Jenkins pull that Code & send to Maven for build.
* once build is done, then jenkins pull that Code and send to Selenium for testing.
* Once testing is done, then Jenkins will pull that code and send to artifactory as per requirement and so on.
* We can deploy with Jenkins.

#### Advantages of Jenkins
* It has lots of plug-ins available.
* You can write your own plug-ins.
* You can use Community Plug-ins.
* Jenkins is not just a tool. It is a framework. i.e. you can do whatever you want all you need is plug-ins.
* We can attach slaves (nodes) to jenkins master. It instruct others (slaves) to do job. If slaves are not available, jenkins itself  does the job.
* Jenkins also bahave as Crone Server Replacement. i.e. Can do scheduled task.
* It can create labels. 
