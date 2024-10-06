#kubernetes #LFS158x 
# Key Features of Kubernetes

## Automatic Bin Packing
Kubernetes automatically schedules or orders containers based on resource requirements and constraints, to maximize utilization without sacrificing availability.
## Designed for Extensibility
Kubernetes Clusters can be extended with new custom features without modifying the upstream source code.
## Self-Healing
Kubernetes automatically replaces and reschedules containers from failed node. It terminates and then restarts containers that become unresponsive to health checks, based on existing rules/policy. It also prevents traffic being routed to unresponsive containers.
## Horizontal Scaling
Kubernetes can manually or automatically scale depending on CPU utilization and other requirements.
## Service Discovery and Load Balancing
Containers are prescribed specific IPs while services are labeled with a single Domain Name System (DNS) entry name to enable load-balancers to manage traffic across nodes and pods.
## Automated Rollouts and Rollbacks
Kubernetes simplifies rollouts and rollbacks for updates or changes while minimizing downtime by monitoring the health of the application.
## Secret and Configuration Management
Kubernetes manages the Secrets and configuration data for applications separately from container images such that images do not need to be rebuilt when a configuration needs to change.
## Storage Orchestration
Kubernetes automatically mounts Software-Defined-Storage (SDS) solutions to containers from sources such as local storage, external cloud providers, distributed storage, and network storage systems.
## Batch Execution
Kubernetes supports batch execution, long-running jobs, and replaces failed containers.
## IPv4/IPv6 Dual-Stack
Kubernetes enables the use of both IPv4 and IPv6 addresses.
# Next
[[Why Use Kubernetes]]?