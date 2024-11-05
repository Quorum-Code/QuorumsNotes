#kubernetes #liveness #readiness #probe
# What are Liveness and Readiness Probes
Liveness and Readiness Probes are a standard used for checking the status of your applications. 
## Liveness or Readiness
Liveness is generally used to see if the application is live, while Readiness is used to see if the application is ready to receive production requests. If restarting will fix an issue the Liveness endpoint should be used, if an issue occurs outside of the pod such as a database dependency is unreachable readiness should fail.
*If the application can be resuscitated it should use the Liveness probe.*
### Configure in a Manifest
The Liveness/Readiness probes can be configured through the element like `spec.container.liveness`.
```
livenessProbe:
  httpGet:
    path: /healthz
    port: 8080
    httpHeaders:
    - name: Custom-Header
      value: Something
  initialDelaySeconds: 3
  periodSeconds: 3
```