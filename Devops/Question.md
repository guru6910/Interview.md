1. what is SDLC (software development life cycle) ?

--> Software Development Life Cycle is a structured process used for software Delivery. The goal of SDLC is to deliver high-quality software that meets customer requirements within a specified timeline and budget. In SDLC common stages are to Define the project's scope, goals, resources, and risks then Requirement for knowing business and technical requirements for the software. later Design in that Create the architecture and detailed design of the software, including databases, interfaces, and system logic then Implementation (Development) to Write the actual code based on the design specifications. then Testing to Test the software for defects, bugs, and ensure it meets the requirements. then after Deployment means Release the software to the production environment for users and Last is Monitoring in that Provide ongoing support, bug fixes, and updates to improve performance or add new features.

--> The Software Development Life Cycle (SDLC) is a step-by-step process that helps teams build high-quality software efficiently. It ensures the software meets customer needs, stays within budget, and is completed on time. Here's a simplified breakdown of its main stages:

- Plan: Decide what the software should do and how to achieve it.
- Requirements: Find out what features and functions the software needs.
- Design: Sketch out how the software will look and work.
- Build: Write the code to create the software.
- Test: Check the software to make sure it works correctly.
- Deploy: Launch the software so people can use it.
- Maintain: Fix issues and improve the software over time

2. explain waterfall methodology.

The waterfall methodology is a sequential approach to software development. In this model each phase the project is completed one by one with no overlap. once the phase is finished you move to the next stage and you cant go back to previous phase easily.

3. Explain Agile methodology.

The Agile methodology is a flexible approach to software development where projects are divided into small, manageable parts called sprints. Teams work in short cycles to create and improve the product based on regular feedback from customers, allowing them to adapt to changes quickly. This helps ensure that the final product better meets user needs.

4. Explain Devops.

DevOps is a set of practices that combines software development and IT operations to improve collaboration, automate processes, and accelerate the delivery of high-quality software. It aims to shorten development cycles and enhance deployment frequency through continuous integration and continuous deployment (CI/CD).

5. what work of devlopers and operations ?

Developers focus on writing code, building features, and fixing bugs in applications, whereas operations (Ops) manage the infrastructure, ensure servers are running smoothly, monitor system performance, and handle deployment. In a DevOps model, both work closely together to streamline the process, automating deployment and ensuring the application runs efficiently in different environments.

6. what is the main purpose of Devops ?

The main goal of DevOps is to improve collaboration between development and operations teams, enabling them to deliver software faster, more reliably, and at higher quality. This is achieved through automation, continuous integration, continuous delivery (CI/CD), and monitoring, leading to shorter release cycles, quicker issue resolution, and a more efficient development process.

7. Explain Git.


8. Explain Github.

GitHub is a web-based platform built on Git that allows developers to host their Git repositories online. It provides tools for collaboration, such as pull requests, issue tracking, and code reviews. GitHub also integrates with other tools to automate workflows, such as continuous integration and deployment, making it easier to manage large projects.

9. Difference between Centralized version control system & Distributed version control system.

In a CVCS, like Subversion (SVN), all version history and project files are stored in a central server, and developers check out files to work on them. If the central server goes down, work is disrupted. In contrast, a DVCS like Git allows every developer to have a full copy of the repository, including its history. This enables faster local commits and offline work, while also reducing the risk of losing project data.

10. Explain staging area.

The staging area in Git is a middle step between modifying files in your working directory and committing them to the repository. You can stage changes selectively, preparing them for a commit, which allows you to break down changes into smaller, more meaningful commits. It’s essentially a “holding” area where you can review and edit what will be included in your next commit.

11. Explain Branching strategy.
12. Explain Environmentin git.
13. what is stash command.

The git stash command temporarily saves your uncommitted changes without deleting them from your working directory. This allows you to switch branches or work on something else, then return and reapply those changes when needed.

14. what is cherry-pick command.

The git cherry-pick command allows you to apply a specific commit from one branch onto another branch without merging the entire branch. It’s helpful when you want to pick out a bug fix or feature from one branch and apply it to another.

15. what is rebase and merge command.
16. what is commit in github.

A commit is a snapshot of your project’s files at a specific point in time. When you make a commit in GitHub, it records what changes were made and by whom

17. what is terraform.

Terraform is an open-source Infrastructure as Code (IaC) tool that lets you define cloud and on-premise infrastructure using configuration files. It allows you to provision and manage resources like servers, databases, and networking components across multiple cloud providers, such as AWS, Azure, and Google Cloud, using a single language. we use also variable and module to reuse code.

18. advantages of terraform.

Terraform is cloud-agnostic, meaning it works with many cloud providers. It supports version control, making it easier to track infrastructure changes. It also enables automated infrastructure management, provides reusable modules, and uses a declarative syntax to define resources, which ensures consistency across environments.

19. Home directory of terraform.

.terraform

20. what is terraform.tfstate file.

The terraform.tfstate file stores the state of your managed infrastructure, mapping real-world resources to your configuration. Terraform uses this file to track changes and decide what actions are required during an apply operation.

21. how to secure tfstate file ?

To secure the tfstate file, you can store it in a remote backend such as AWS S3, which supports encryption and access control. 

22. what is API ?

An API (Application Programming Interface) is a set of rules and protocols that allows different software systems to communicate with each other. It defines how requests and responses should be formatted, enabling different applications to interact, such as a mobile app fetching data from a server.

23. difference between coludformation and terraform.

CloudFormation is an AWS-specific Infrastructure as Code tool, whereas Terraform is cloud-agnostic and can be used with multiple cloud providers. Terraform’s configuration language is more flexible and allows for reusable modules, while CloudFormation is tightly integrated with AWS services but limited to that ecosystem.

24. difference between Ansible and terraform.

Ansible is used for configuration management and automating tasks on existing infrastructure, while Terraform is used for provisioning infrastructure. Ansible configures and manages resources, whereas Terraform creates and manages the underlying infrastructure resources like VMs and networks.

25. Explain all block in terraform.

Terraform configuration files are built using blocks. The key blocks are:

provider: Specifies the cloud provider (e.g., AWS, Azure).
resource: Defines the actual infrastructure (e.g., EC2 instance).
variable: Defines input values that make your configuration more flexible.
output: Defines values you want to display after the apply phase, like server IPs.
data: Allows you to reference existing resources.

26. what is variable in terraform ?

A variable in Terraform is used to make configurations flexible and reusable. It allows you to input dynamic values, which can be passed during runtime, making it easy to manage different environments with the same codebase.

27. what is module in terraform ?

A module in Terraform is a reusable block of code that can be shared across configurations. It helps organize resources logically and allows you to reuse infrastructure setups across projects.

28. Explain Provisioner in tf ?

Provisioners in Terraform are used to execute scripts or commands on a resource after it has been created. For example, you can use a provisioner to install software on a virtual machine after Terraform provisions it.

29. explain datablock.

The data block in Terraform allows you to reference existing resources in your configuration. For instance, if an EC2 instance already exists, you can use the data block to retrieve its details without creating a new instance.

30. what is ansible and what we use it ?

Ansible is an open-source tool used for configuration management, application deployment, and task automation. It simplifies managing multiple servers by automating repetitive tasks, such as software installation, system updates, and environment setup.

31. what is inventory file ?

The inventory file lists the servers (hosts) that Ansible will manage. It can include groups of hosts, making it easier to manage large infrastructures by grouping servers based on environment or function.

32. what is playbook file ?

A playbook in Ansible is a YAML file that contains a list of tasks. These tasks define what actions should be taken on the hosts listed in the inventory file, such as installing software, copying files, or starting services.

33. what is mean b ansible hosts ?

 In Ansible, hosts refer to the target machines on which you want to run Ansible tasks. These hosts are specified in the Ansible inventory file and can be individual servers or groups of servers. For example, if you want to deploy an application across multiple web servers, you would list those servers as hosts in your inventory. Ansible then applies the defined tasks in your playbook to these hosts.
 
34. what is the configuration path of ansible ?

`/etc/ansible/ansible.cfg`

35. what is variable in ansible ?

Variables in Ansible allow you to store and reuse data across playbooks, roles, and tasks. They make playbooks more dynamic and flexible by abstracting values like paths, configuration details, or environment-specific settings. You can define variables in inventory files, playbooks, or group/host-specific files.

36. what is module in ansible ?

A module in Ansible is a standalone script that performs a specific task, such as installing packages, managing files, or handling services. Ansible comes with many pre-built modules, such as yum (for installing packages on Red Hat-based systems), copy (for copying files), and user (for managing users). You can also write custom modules if needed.

37. what is docker ?

Docker is a platform that automates the deployment of applications inside lightweight, portable containers. It allows you to package your application, along with its dependencies, into a container that can run consistently across various environments, ensuring that "it works on my machine" is no longer a problem.

38. why we use docker ?

Docker makes development, testing, and deployment easier by using containers that create the same environment everywhere. Containers are lightweight, portable, and run consistently on any system. Docker also helps apps scale quickly, keeps resources separate, and uses less system power than traditional virtual machines.

39. what is image in docker ?

A Docker image is a lightweight, stand-alone, executable package that contains everything needed to run a piece of software, including the code, runtime, libraries, and system tools. Images are read-only templates used to create containers.

40. what is container in docker ?

A Docker container is a runtime instance of a Docker image. It is a lightweight, standalone, and executable package of software that includes everything it needs to run. Unlike virtual machines, containers share the host OS's kernel but run in isolated environments.

41. what is dockerfile ?

A dockerfile is a text file that contains set of instructions for building a docker image. It defines the base image, dependencies, configuration settings, and commands to be executed when the image is built. For example, it might define which version of an operating system or programming language should be installed.

42. componants of dockerfile ?

- FROM: Specifies the base image.
- RUN: Executes commands during the build process.
- COPY/ADD: Copies files from the host system to the container.
- WORKDIR: Sets the working directory inside the container.
- CMD/ENTRYPOINT: Defines the command to run when a container starts.
- EXPOSE: Specifies the port that the container will listen on.
- ENV: Sets environment variables inside the container.

43. what is mean by docker engine ?

Docker Engine is the core component of Docker that allows you to build and run containers. It consists of the Docker daemon, which manages Docker containers, images, and networks, and the Docker CLI (command-line interface), which allows you to interact with Docker.

44. why do we use docker ?

Docker is used because it provides a lightweight, scalable, and consistent environment for running applications. Containers are fast to start, use fewer resources compared to virtual machines, and help in creating reproducible development environments. Docker also enables easier collaboration, CI/CD pipelines, and faster deployment.

45. Architecture of Docker.



46. how many digit in git commit id ?

A Git commit ID (hash) is a 40-character long string.

47. diffrence between virtual machine and local machine.

A local machine refers to your physical computer that runs your operating system and applications directly. A virtual machine (VM) is an emulation of a physical computer that runs an operating system and applications inside a host machine using a hypervisor. Virtual machines provide isolation from the host system, whereas a local machine runs everything natively.

48. difference between virtual machine and container.

Virtual Machine: Has its own OS and runs on a hypervisor, consuming more resources and being slower to boot.
Container: Shares the host system's OS kernel, making it lightweight and faster to start. Containers use fewer resources compared to VMs as they only virtualize the application layer, not the entire OS.

49. what is docker compose file in docker ?

A Docker Compose file (typically named docker-compose.yml) is used to define and manage multi-container Docker applications. It allows you to define services, networks, and volumes in a single YAML file, making it easier to manage containers in complex applications.

50. what does docker networking ?

Docker networking allows containers to communicate with each other, the host system, and external networks. It manages how containers connect and share data, both inside and outside the Docker environment. 

51. explain all types of networking ?

there are 5 type of docker network first one is Bridge , it is a default network in docker Containers in the same bridge network can communicate with each other, but they are isolated from containers on other networks. then after Host Network The container shares the host system's network. It directly uses the host's IP address.
There is no network isolation between the container and the host. then None Network it Completely disables networking for the container.
The container has no network interface. later Overlay Network Used for communication between containers across different Docker hosts in a Swarm or Kubernetes environment. It enables multi-host networking. and last is Macvlan Network it Assigns a unique MAC address to containers, making them appear as physical devices on the network. in that Containers can be treated as separate devices by the network.

52. what is docker volume ?

A Docker volume is a storage mechanism that allows data to persist beyond the life of a container. Volumes store data outside of the container's filesystem, making it possible to retain data even if the container is stopped or deleted. Volumes are commonly used when you need to store logs, databases, or configuration files that should survive container restarts

53. what is k8s and why we use it ?

K8s (Kubernetes) is an open-source platform for automating the deployment, scaling, and management of containerized applications. It orchestrates containers, ensuring that your applications run smoothly across multiple environments. Kubernetes simplifies the management of large-scale containerized applications, making them easier to deploy, scale, and maintain.

**Why We Use Kubernetes:**
Automated Deployment: Kubernetes automates the deployment of applications in containers, reducing manual work.
Scalability: It automatically scales applications up or down based on demand, ensuring efficient use of resources.
Self-Healing: If a container fails, Kubernetes can restart it or replace it, ensuring high availability and reliability.
Load Balancing: Kubernetes distributes traffic across containers to maintain performance and prevent overload.
Portability: Since it works with containers, Kubernetes can run applications consistently across different environments (on-premise, cloud, hybrid).

54. Architecture of kubernetes ?



55. what does kube schedular in kubernetes ?

The Kube Scheduler in Kubernetes is responsible for assigning newly created pods to nodes in the cluster. When a pod is created but not yet assigned to a node, the scheduler decides which node the pod should run on, based on various factors like resource availability, load, and any specific scheduling constraints or policies.

56. what does kube-proxy in k8s ?

Kube-proxy is a network component in Kubernetes that manages network communication inside and outside of the cluster. It handles network traffic and ensures that each service can be reached by the right pods.
 Kube-proxy manages network traffic in Kubernetes, helping services and pods communicate efficiently within the cluster.

57. Advantages of kubernetes ?

Kubernetes offers several key advantages that make it a powerful tool for managing containerized applications: 
- Automated Scaling
- Self Healing
- Load Balancing
- Atomated Rollout and Rollbacks
- Portability
- Load Balancing
- Secret and Configuration Management
- Support Multiple Workloads

58. what is eks cluster ?

An EKS (Elastic Kubernetes Service) cluster is a managed Kubernetes service provided by AWS (Amazon Web Services). It simplifies the process of deploying, managing, and scaling Kubernetes applications in the cloud.

59. what is lable ?

In Kubernetes, a label is a key-value pair that is attached to objects like pods, services, and deployments. Labels are used to organize and categorize these objects, making it easier to manage and select groups of resources based on specific criteria.

60. explain selector and type of selector ?

In Kubernetes, a selector is a mechanism used to identify a set of resources (like pods) based on their labels. Selectors help you query and manipulate groups of objects efficiently.

61. explain type of set based selector ?

there are two type of selectors first one is Equality Based Selector These selectors match resources based on exact label values. Syntax: `key=value` and Second one is Set based Selectors These selectors allow you to match resources based on a set of values for a given key. in that also three type IN, NOTIN and EXITS. 
- In = key: value
- NotIN = key: value : avoid it and run
- Exists = env{ } : run all which hav in that env

62. what is pod explain in brief ?

A pod is the smallest deployable unit in Kubernetes that can contain one or more containers. Pods share the same network namespace, which means they can communicate with each other using localhost. They also share storage volumes, allowing containers within a pod to access the same data. Pods are designed to run a single application or service and are managed by Kubernetes for scaling, health checks, and networking.

63. what is Replication controller ?

A Replication Controller in Kubernetes ensures that a specified number of pod replicas are running at all times. It monitors the pods and automatically creates or deletes them to maintain the desired count, providing high availability and scaling for applications. While it's been largely replaced by ReplicaSets in newer versions, it still functions to manage pod lifecycles effectively.

64. what is Replica set ?

A ReplicaSet in Kubernetes is a resource that ensures a specified number of pod replicas are running at all times. It automatically manages the creation and deletion of pods to maintain the desired count, providing high availability and scalability for applications. ReplicaSets can also help facilitate rolling updates by managing the transition of pods during updates, ensuring that the application remains available.

65. how we manage pod in k8s ?

we can manage the pod with several key actions like creating pods, Deleting pods, scaling pods, updating pods, monitoring pods, check the logs of pods, and Health check the pods By using these methods, you can effectively manage the lifecycle, availability, and performance of your pods in Kubernetes.

66. difference between RC & RS.

## Replication Controller:
- Older Resource: It was the original mechanism for managing pod replicas in Kubernetes.
- Basic Functionality: Ensures the desired number of pod replicas but has limited features compared to ReplicaSets.
- Label Selector: Uses a simple equality-based selector to match pods, making it less flexible for complex deployments.
## ReplicaSet:
- Newer Resource: Designed to replace Replication Controllers with improved functionality.
- Enhanced Selector: Supports both equality-based and set-based selectors, allowing for more complex matching of pods.
- Integration with Deployments: Typically used in conjunction with Deployments to manage rolling updates and maintain application availability.

67. what is Deploymwnt and why we use it ?

A Deployment in Kubernetes is a higher-level abstraction that manages the lifecycle of applications by defining how many replicas of a pod should run, as well as the updates to those pods. Deployments provide a robust way to manage application updates, scaling, and availability in Kubernetes. We use deployment for basically for Easy Rollout and Rollbacks, Declarative Updates, Scalling, Health Monitoring, Replica Management. 

68. why we use strategy in deployment ?

In Kubernetes, strategies in deployments are used to control how updates to applications are managed. They ensure that updates happen smoothly, minimizing downtime and maintaining availability. For example, rolling updates gradually replace old pods with new ones, which helps prevent service disruptions. If something goes wrong during an update, strategies enable quick rollbacks to a previous stable version. Additionally, they can include health checks to ensure new pods are functioning correctly before directing traffic to them. Overall, deployment strategies provide greater reliability and control over application updates.

69. what happend when we use rolling update strategy ?

When using a rolling update strategy in Kubernetes, the deployment gradually replaces old pods with new ones without downtime. it replace old version to new version pods one by one.

70. what happened when we us recreate strategy ?

When you use the recreate strategy in a Kubernetes deployment, all existing pods are terminated before new pods are created. This means that there will be a period during which the application is unavailable, as the old pods are shut down and the new ones are brought up. it that between have a downtime.

71. explain blue-green , A-B testing strategy in brief.

**Blue-Green** Deployment is a strategy where two identical environments, called "blue" and "green," are maintained. At any given time, one environment is live (serving users), while the other is idle. When a new version of the application is ready, it is deployed to the idle environment. Once tested, traffic is switched to this environment, minimizing downtime and risk. If issues arise, you can quickly revert to the previous environment.

**A/B Testing** involves deploying two versions of an application (A and B) simultaneously to different user segments. This allows you to compare performance, user engagement, or other metrics to determine which version is more effective. It helps in making data-driven decisions about features or improvements based on real user feedback.

72. difference between statefulset and statelessset.

**StatefulSet** is designed for applications that require stable, unique network identifiers and persistent storage. Each pod in a StatefulSet has a unique identity and maintains its state across restarts. This is useful for applications like databases, where data consistency and identity are crucial.

**stateless** deployment (like a Deployment) is for applications that don’t need to maintain any state between sessions. Pods can be created and destroyed at any time without affecting the application's functionality. They are interchangeable, meaning any pod can handle any request.

73. difference between statefulset and deployment.

 

74. what is namespace and why we use it in k8s ?

A namespace in Kubernetes is a way to group and organize resources. It helps separate different projects or environments within the same cluster, so teams can work without interfering with each other. Namespaces make it easier to manage resources and apply security rules, allowing for better organization and control. Using namespaces improves resource management, enhances security through access control, and enables better organization of environments (like development, testing, and production) within the same cluster.

75. what is the default namespace ?

The default namespace in Kubernetes is simply called "default." When you create resources like pods or services without specifying a namespace, they are placed in this default namespace. It's a convenient way to organize resources if you don't need multiple namespaces for isolation. and also we can change the default namespace.

76. what is the service in k8s ?

A Service in Kubernetes is an abstraction that defines a logical set of pods and a policy for accessing them. Services provide a stable endpoint (IP address and DNS name) for accessing a group of pods, even as those pods are created or destroyed. This allows applications to communicate with each other reliably. Services can also enable load balancing and can be configured to expose applications internally within the cluster or externally to the outside world. They come in several types, such as ClusterIP (default, for internal access), NodePort (for external access), and LoadBalancer (for cloud environments).

77. type of service ?

There are four type of Services first one is ClusterIP it Exposes the service internally within the cluster. It can't be accessed from outside.
then NodePort is Exposes the service on a static port on each node's IP, allowing external access. then after LoadBalancer to Creates an external load balancer (in cloud environments) to distribute traffic and provide a single IP for access and last is ExternalName for Maps the service to an external DNS name, allowing access to external resources using a Kubernetes service name.

78. what is daemonset ?

A DaemonSet in Kubernetes ensures that a specific pod runs on all or selected nodes in the cluster. It's used for tasks like logging or monitoring, automatically scheduling pods on new nodes and cleaning them up when nodes are removed.

79. what is volume ?

A volume in Kubernetes is a way to store data that lasts beyond the life of a pod. It allows data to persist and be shared between pods, even if the pods are deleted or restarted. Volumes can use various storage types, like local disks or cloud storage.

80. type of volume ?

- emptyDir: A temporary storage that lasts as long as the pod is running. It’s created when the pod starts and deleted when it stops.
- hostPath: Mounts a file or directory from the host node's filesystem into the pod. Useful for accessing files on the host.
- PersistentVolume (PV): A storage resource in the cluster that is provisioned by an administrator and can be used by pods. It provides a way to manage storage independently of pods.
- PersistentVolumeClaim (PVC): A request for storage by a user. It binds to a specific PersistentVolume based on storage needs.

81. what is pv and pvc ?

PersistentVolume (PV) is a storage resource in a Kubernetes cluster that has been provisioned by an administrator. It represents a piece of storage that can be used by pods. And PersistentVolumeClaim (PVC) is a request made by a user for storage. It specifies the amount of storage needed and can bind to an available PersistentVolume that meets the criteria. PVCs allow users to dynamically claim storage resources without needing to know the details of the underlying storage infrastructure.

82. what is emtydir ?

emptyDir is a type of volume in Kubernetes that provides temporary storage for a pod. It is created when the pod is assigned to a node and exists as long as the pod is running. When the pod is deleted or stopped, the data stored in the emptyDir volume is lost.

83. what is Hostpath ?

hostPath is a volume type in Kubernetes that mounts a file or directory from the host node's filesystem into a pod. This allows the pod to access files or directories on the host system directly. It's useful for scenarios where you need to share data between the host and the pod or when you want to access specific resources on the host.

84. explain Access modes in volume ?

There are three main access modes: first one is ReadWriteOnce (RWO) in that The volume can be mounted as read-write by a single node. This is the most common mode, allowing one pod on one node to write to the volume later second is ReadOnlyMany (ROX) it The volume can be mounted as read-only by multiple nodes. This means several pods can read from the volume simultaneously, but none can write to it and third is ReadWriteMany (RWX) in that The volume can be mounted as read-write by multiple nodes. This allows multiple pods across different nodes to write to the volume, making it useful for shared storage scenarios.

85. explain Persistent Volume Reclaim Policy ?

This policy determines what happens to a PersistentVolume (PV) when its associated PersistentVolumeClaim (PVC) is deleted there is three type of persistent volume reclaim policy first one is Retain for The PV is not deleted. it not reuse with another pv then Delete policy for The PV and its data are deleted along with the PVC. This is useful for dynamic provisioning then after Recycle policy for The PV’s data is scrubbed (basic data wipe) and the PV is made available for a new claim.

86. what is configmap ?

A ConfigMap in Kubernetes is an object that allows you to store configuration data as key-value pairs. It is used to separate configuration settings from application code, making it easier to manage and update configurations without changing the codebase. Store non-sensitive configuration data in key-value pairs.

87. what is secret ?

Secrets are used to store sensitive information such as passwords, OAuth tokens, SSH keys, and TLS certificates. Secrets can be mounted as volumes in Pods, allowing applications to read sensitive data from the filesystem securely. Store and manage sensitive passwords or API keys used by applications. Manage encryption keys required for securing application data.

88. what is ingress in k8s ?

Ingress in Kubernetes is a resource that manages external access to services within a cluster, typically HTTP and HTTPS traffic. It provides routing rules to direct incoming requests to the appropriate service based on the request's URL or host.

89. why we use ingress ?

We use Ingress in Kubernetes to manage how external users access services inside the cluster. It allows us to route web traffic based on URLs, use a single IP address for multiple services, and handle secure connections easily. Essentially, Ingress simplifies and organizes how external requests reach our applications.

90. explain jenkins.

Jenkins is an open-source automation server that helps automate the process of building, testing, and deploying software. It supports continuous integration and continuous delivery (CI/CD), allowing developers to frequently merge their code changes into a shared repository. Jenkins helps teams to deliver software faster and with higher quality by automating repetitive tasks in the development lifecycle. In that we manage plugins then pipeline automation.

91. what is the home directory path of jenkins ?

The default home directory path for Jenkins is usually /var/lib/jenkins. This is where Jenkins stores its configuration files, job data, build artifacts, and plugins.

92. explain plugin in jenkins.

Plugins in Jenkins are add-ons that enhance the functionality of the Jenkins server. They allow users to integrate with various tools and services, automate tasks, and extend Jenkins features. With plugins, you can Integrate with Version control systems like Git then building tools like maven, later Deployment tools and CI/CD Enhancement

93. what is credential in jenkins ?

In Jenkins, credentials are secure information that can be used by jobs and pipelines to authenticate against external systems or services. They can include usernames, passwords, API tokens, SSH keys, and more.

- Store credentials securely.
- Use them in pipelines and jobs without exposing sensitive information.
- Configure different types of credentials, like username/password pairs or secret files.

94. what is tool configuration in jenkins ?

Tool configuration in Jenkins refers to the process of setting up and managing various development, build, and testing tools that Jenkins pipelines and jobs can use. These tools are typically external utilities or software required by Jenkins to perform certain tasks such as compiling code, running tests, or deploying applications. we add in that tools such as JDK, maven, Git, Docker and SonarQube Scanner.

95. explain Node in jenkins.

In Jenkins, a Node refers to a machine, either physical or virtual, that Jenkins uses to run jobs or pipelines. Nodes can be the master node (now called controller) or agent nodes. Agents are connected to the master through various protocols (like SSH or JNLP). Each node can have specific labels, which allow you to assign jobs to specific agents based on their capabilities.
- Master Node (Controller):

The main Jenkins server or controller node is responsible for scheduling jobs, dispatching jobs to agent nodes for execution, and managing Jenkins resources and configurations.
It also handles user requests, plugin management, and provides the web interface.
- Agent Node:

Agent nodes are machines that perform the actual work of building, testing, and deploying projects.
The agent communicates with the master, accepts job instructions, executes them, and reports the result back to the master.
You can have multiple agent nodes to distribute workloads and execute jobs concurrently on different platforms or environments.

96. what is pipeline ?

In Jenkins, a Pipeline is a suite of plugins that supports the implementation and automation of continuous delivery pipelines. It allows you to define the entire lifecycle of your software development process, from building and testing to deploying the application, in the form of code. A Jenkins pipeline is defined in a Jenkinsfile, which is a text file that contains the pipeline's definition. 

97. what is type of pipeline ?

The Jenkins pipeline has two main types:

**1. Declarative Pipeline:** 
A higher-level, more readable syntax designed for users who may not be deeply familiar with Groovy (the language Jenkins pipeline is based on). The pipeline is defined inside a pipeline block and typically includes stages like build, test, and deploy.

**2. Scripted Pipeline:** 

Offers more flexibility and is fully written in Groovy. It is a lower-level syntax that provides more control, but is more complex compared to the declarative style.


98. resource in terraform.

In Terraform, a resource is a key building block that defines infrastructure components such as servers, databases, load balancers, or any service you want to create and manage. Resources represent objects in your infrastructure, and by declaring them in your Terraform configuration files, you instruct Terraform to manage those objects.

99. what is cluster ip ?

In Kubernetes, a ClusterIP is a type of service that provides internal access to a set of Pods in the cluster. It is the default service type in Kubernetes and exposes the service on an internal IP address that is accessible only within the cluster.

100. what is terraform import command ?

The terraform import command lets you bring existing infrastructure under Terraform's management without changing it. It updates Terraform's state file so that Terraform can track and manage resources created outside of Terraform.

101. what is taint command in terraform ?

The main reason to use the Terraform taint command is to mark a resource (such as an EC2 instance) as being in a bad or non-functional state. This ensures that it will be destroyed and recreated in the next terraform apply.

102. why container is lightwated ?

Containers are lightweight because they share the host OS kernel, avoiding the overhead of multiple operating systems. They start quickly, use fewer resources, and leverage a layered file system for efficiency.

103. what is docker community edition and enterprise edition ?

Docker Community Edition (CE) is a free, open-source version for individual developers, offering basic features and community support. Docker Enterprise Edition (EE) is a paid version for organizations, providing advanced features, commercial support, and enhanced security for production environments.

what is terraform locate 
what is multistage container 
