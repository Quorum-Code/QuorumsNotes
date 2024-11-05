#kubernetes #resource-requests #resource-limits
# What are Resource Requests and Limits
Resource Requests and Limits control the amount of either memory or CPU m (millicores) reserved or used by a pod.
## Resource Requests
The resource request is a configuration to enforce the minimum resources required to spin up a pod, this can be arbitrary and is not calculated.
*If a memory or CPU resource requested is not available, a pod will not be spun up.*
## Resource Limits
The resource limit configures the maximum amount of millicores or memory used allocated to a pod. 
*If an amount of memory is not available, pod will crash. If an amount of millicores is not available will only slow down the pod.*
### Millicores and Memory Units
Millicores are whole numbers followed by a lower-case 'm', `1000m` is equal to one core. 
The units for Memory are a whole number followed by the upper-case first letter of a standard unit of computer memory then a lower-case 'i', `300Mi` is equal to 300MiB (Mebibyte).
The above are only some of the valid formats for units, more can be found [here](https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/#meaning-of-cpu). 
## Statuses
* `OOMKilled` - Out of Memory Killed, 