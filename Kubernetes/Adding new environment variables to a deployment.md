#kubernetes

1. Create a configmap with env vars (note the configmap metadata name)
2. List deployments
3. Edit deployment using `kubectl edit deployment [deployment name]` then to `spec.template.spec.containers`, to the container you would like to provide env vars add `envFrom: - configMapRef: name: [configmap metadata name]`