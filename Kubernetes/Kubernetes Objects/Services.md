#kubernetes #services 
# What is a Service
Services enable accessing pods through a name (effectively a pseudo DNS record). Which allows for load balancing and reliability because a does not lock into a single IP address.
## Creating a Service
```
kind: Service
metadata:
  name: myboot
  labels:
    app: myboot
spec:
  ports:
  - name: http
    port: 8080
selector:
  app: myboot
type: LoadBalancer
```
This is a manifest for creating a Load Balancing Service which is configured for pods with the label `app=myboot`. 
## Getting all Services
`kuebctl get svc`
This will print out services with their port, which is necessary to reach the service. In the listings under the `PORT(S)` column the values are application port (port) and exposed port (target/listening port).
## Testing a Load Balancing Service
`while true; do curl <Node-IP>; sleep .5; done`
Will curl the pod applications (pods can be set up to respond with their pod-name with hash to be able to tell that different pods are being reached with each curl). 