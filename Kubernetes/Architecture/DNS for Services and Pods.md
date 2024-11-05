#kubernetes 

# Internal DNS Routing

Kubernetes automatically generates DNS entries for Services and Pods. DNS entries are generated as such, `<namespace>.svc.cluster.local`. Namespace is optional, it is otherwise assumed to be the Namespace of whichever Pod is from. 