#kubernetes #label
# What is a Label
A Kubernetes label is a key value pair which is attached to Kubernetes objects and can enable simple control of many objects at the same time.
## Viewing Labels
`kubectl get pods --show-labels`
The show-labels options will print out all the labels for the objects being retrieved.
## Control by Label
`kubectl delete pods -l <labelname>=<labelvalue>`
This command will delete all pods which have the label of `labelname` with a value of `labelvalue`.
## Manually Adding a Label
`kubectl label pods -l <existinglabelkey>=<existinglablevalue> <newlabelkey>=<newlabelvalue>`
Will add the new label pair to any pods which have the existing label pair.