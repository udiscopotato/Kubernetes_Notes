### What's the purpose of Kubernetes ?
The purpose of Kubernetes is to host your applications in the form of containers in an automated fashion so that you can easily deploy and manage as many instance of your application, and enable service communication between them.

### Docker vs ContainerD
Docker is a comerhensive platform which provides tools for building, running, managing and distributing containers. It includes various components like docker cli, docker enginer, docker swarm, docker compose etc. whereas ContainerD is an industry standard container runtime created by docker and later donated to CNCF. It designed to handle low level container runtime tasks effectively.
ContainerD is more modular and lightweight compare to docker that's why it's used in many orchestrators tools and even docker itself.

### What's a pod ?
A pod is the smallest unit of deployment in Kubernetes, and is made up of one or more containers that run instances of an application. Pods are the fundamental building blocks of Kubernetes workloads, and are hosted inside nodes in a cluster.

### What's a pod definition file ?
A pod definition file is a declarative YAML file that defines a Kubernetes pod.

### What's the difference between pod and container ?
A container is a isolated, lightweight, portable and executable software package that include everything that need to run a application i.e. library, dependancy, etc. Whereas A pod is the smallest deployable unit in Kubernetes. It represents a group of one or more containers that are deployed together on the same host.
All containers within a pod share the same network namespace, IP address, and port space. They can communicate with each other using localhost.

### What's ReplicaSet ?
A ReplicaSet is a Kubernetes Object responsible for ensuring that a specified number of pod replicas are running and operational at any given time. It helps to achieve high availability and scalability for your applications by managing the lifecycle of pods.

### ReplicationController  vs  ReplicaSet
They both have the same purpose but they're not the same. Both are used for running and maintaining a specified number of identical pod replicas
Replication Controller is the older technology that got replaced by ReplicaSet, it is the new recommended way to setup replication.
ReplicaSet is an improved version of ReplicationController with additional features like better selector support and support for rolling updates. 

### Why do we use labels and selectors in kubernetes ?
Labels and selectors are fundamental concepts in Kubernetes that enable flexible and efficient management of resources within the cluster.
- Grouping and organizing resource.
- Service Discovery and Load Balancing.
- Targeting Resources.
- Monitoring and Observability.
- Managing Access and Policies.
