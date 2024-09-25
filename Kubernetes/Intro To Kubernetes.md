#kubernetes 

# What is Kubernetes

Kubernetes is a tool to control many [[Containers]] with one system.

The Kubernetes platform controls a Kubernetes Cluster. A Kubernetes Cluster is made up of one or many worker nodes. [Control Plane Components](https://kubernetes.io/docs/concepts/overview/components/#control-plane-components) manage the overall state of the cluster. [Node Components](https://kubernetes.io/docs/concepts/overview/components/#node-components) run on every node, maintaining running pods, and providing the Kubernetes runtime environment.
# Why use Kubernetes

* Kubernetes can manage [[Load Balancing]]. 
* Orchestrate storage through [[Volumes#Persistent Volumes (PV)|Persistent Volumes]].
* Automatic Rollouts and Rollbacks. 
* Automatic bin packing.
* Self-healing [[Containers]] in response to user-defined checks.
* Management of secrets and configurations.
* Batch execution.
* Horizontal scaling.
* IPv4 and IPv6 dual-stack.

# Kubernetes Object Management

## Objects in Kubernetes

Kubernetes Objects are a "record of intent", some specification is created by the user and the Kubernetes system attempts to populates its cluster according to those specifications. Kubernetes Objects are created, modified, and deleted using the Kubernetes API, in the CLI you can use `kubectl` to perform calls to the API for you. When using `kubectl` you usually provide `.yaml` files which are called [[Manifests]] in the Kubernetes framework.

## Some Points
* K8s is an alias for Kubernetes
* Highly scalable
* Kubernetes is a distributed system of servers that host software applications, and you interact with it primarily through your local command line.
* Progressive rollouts
* Load balancing
* Container orchestration tool
