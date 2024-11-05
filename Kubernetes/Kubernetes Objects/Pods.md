#kubernetes #pods
# What is a Pod
Pods are the smallest deployable units of computing that you can create and manage in Kubernetes. It is a group of one or more [[Containers]], with shared storage and network resources, and a specification for how to run the containers. A Pod always runs its [[Containers]] in a shared context, effectively running on the same logical host, where applications or processes are tightly coupled. Simply put, everything within a Pod is running similarly to how processes would run on one machine. 

*Pods shouldn't be used directly. Pods are supposed to be a unit that is managed, so if you create a pod you have to manage it, its better to create a deployment or some other object that will create pods and manage them automatically.*

# Pod Dogma
Pods are relatively ephemeral, meaning they are disposable. The user handles the Kubernetes API and the API handles the Pods.

A Pod persists until it is deleted. A Pod can be deleted by a user, when it is evicted for lack of resources, or the node its on fails. *A restart does not delete the state of the Pod.*
# Single Container Pod Model
The most common use case for Pods is one container per Pod. 
# Multi Container Pod Model
The less common use case for Pods is for many containers . 

*SHOULD NOT BE USED FOR REDUNDANCY OR CAPACITY! 
Should only be used when containers are tightly coupled.*

## Pods vs. Containers
Below is an example of **3 pods running 3 total containers (synergychat-web)** and **1 pod running 3 containers (synergychat-crawler)**.
`
```
synergychat-crawler-5464f9b774-nt9qc   3/3     Running   0          31s
synergychat-web-598b96dcff-259rg       1/1     Running   0          3h42m
synergychat-web-598b96dcff-ngmj7       1/1     Running   0          3h42m
synergychat-web-598b96dcff-sbpcw       1/1     Running   0          3h42m
```

## What can cause a Pod to be deleted
* The node they're running on fails
* A new version of the image was published
* A new node was added to the cluster and the pod was rescheduled