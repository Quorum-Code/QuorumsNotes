#kubernetes #yaml #json

# What is a Manifest

A Manifest is a file that specifies details about a Kubernetes Object. The common format is [[YAML]] but JSON format works as well.

Manifests are often used with `kubectl apply -f [MANIFEST]`, which can create a Deployment, Service, or something else defined in that Manifest.

# Required Fields

## `apiVersion`

The version of the Kubernetes API you're using to create this object. (Often the desired value is `v1`).

## `kind`

The kind of object you want to create.

## `metadata`

Data that helps a user identify the object such as `name`, `UID`, and `namespace` optionally.
## `spec`

Specification of the desired state of the object to be created.