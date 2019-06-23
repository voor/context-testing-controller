# Context Testing Controller

This is a very simple controller made with most of the defaults from [kubebuilder](https://book.kubebuilder.io/quick-start.html), modified to add in the appropriate Pod Security Policy to run in a high security environment.

## Getting Started

You are most likely not that interested in the go aspects of this repository, and instead just want to play around with a controller that applies different Pod Security Policies for its created CRD deployments.

If that is the case, you don't need to build this controller at all, and it's provided at Docker hub already, and similarly applied into the deployment configuration here.

Just clone this repository, make sure your `kubectl` is pointing to a cluster with the PSP Admission Controller, and run:

```
kubectl apply -f security-context.yaml 
```