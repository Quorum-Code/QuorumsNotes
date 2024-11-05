#kubernetes #namespaces
# What is a Namespace

[Namespaces](https://kubernetes.io/docs/concepts/overview/working-with-objects/namespaces/) are a tool to keep Kubernetes systems organized and a way to isolate cluster resources into groups, those resources being Kubernetes objects. 

Namespaces impact [[DNS for Services and Pods]]. 

`kubectl get namespaces`
`kubectl get ns`

# Namespaces and `kubectl`

A user can specify the desired namespace with `kubectl -n [NAMESPACE] [TERMS]...`. Default is the assumed namespace if the namespace option is not used.

# [Initial Namespaces](https://kubernetes.io/docs/concepts/overview/working-with-objects/namespaces/#initial-namespaces)

## `default`

The assumed namespace when none are provided.

## `kube-node-lease`

Holds Lease objects associated with each node. Used for the control plane so it can detect the current state of nodes and objects.

## `kube-public`

Readable by all clients authenticated or not. Mostly reserved for cluster usage for any resources that should be visible and readable throughout the whole cluster.

## `kube-system`

For objects created by the Kubernetes system.

## Commands

`kubectl create ns [NAMESPACE]`
`kubectl get ns`