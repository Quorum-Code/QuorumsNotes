#kubernetes 

## Local Storage
Pods have access to local filesystem, but the files are ephemeral. So they are deleted when a pod is restarted or deleted.

## Persistent Storage
[[Kubernetes Volumes]] provide Data Persistence and Data Sharing across containers.
(Volumes can be created to be ephemeral when the sole purpose is to share data between containers)

## Persistent Volumes (PV)

Persistent Volumes are a cluster-level resource that is created separately from pods and then attached to the pods. Somewhat similar to [[Config Maps]].

Statically or dynamically created.
* Static PVs are created manually by a cluster admin
* Dynamic PVs are created automatically when a pod requests a volume that doesn't yet exist
* *Dynamic PVs are more often used in cloud environments.*

### Persistent Volume Claims (PVC)

[Persistent Volume Claims](https://kubernetes.io/docs/concepts/storage/persistent-volumes/#persistentvolumeclaims) is a request for a persistent volume. When using dynamic provisioning, a PVC will automatically create a PV is one doesn't exist that matches the claim. The PVC is then attached to a pod, just like a volume would be.

### Persistent Volume Claim Example

The following is the YAML configuration for a simple PVC.

```
apiVersion: v1
kind: PersistentVolumeClaim
metadata:
  name: synergychat-api-pvc
spec:
  accessModes:
    - ReadWriteOnce
  resources:
    requests:
      storage: 1Gi
```

* `1Gi` requests 1GB of storage space.

Apply the PVC with `kubectl apply -f [filename]`.

List the active PVCs with `kubectl get pvc`.

List the existing PVs with `kubectl get pv`