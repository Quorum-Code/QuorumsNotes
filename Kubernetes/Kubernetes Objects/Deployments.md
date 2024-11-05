#kubernetes #deployments
# What is a Deployment
A deployment contains a replica set and maintains the history of configurations used, this enables rolling back and rolling forward.
## Updating the Deployment Manifest
## Viewing the Deployment History
`kubectl rollout history <deploymentname>`
## Rolling back 
`kubectl rollout undo <deploymentname> --to-revision=<#>`
Provide the deployment name and the revision number from the history to rollback to a specific state.