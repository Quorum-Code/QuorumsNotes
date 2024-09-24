#kubernetes 

Pods can run one or multiple containers.
## Pods vs. Containers

Below is an example of **3 pods running 3 containers (synergychat-web)** and **1 pod running 3 containers (synergychat-crawler)**.
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