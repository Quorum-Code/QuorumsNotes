#kubernetes 

# Databases and Clusters

It is possible to set up databases within Kubernetes but it is not the easiest task. Requires things like, creating persistent volumes, handling Postgres version updates, setting resource limits, and setting up automated backups.

# Use Case for Databases on Kubernetes

A possible use case for databases on Kubernetes is when the database is not mission critical, like live metrics that don't necessarily need to be stored forever but are just used for interesting graphs or development monitoring.

