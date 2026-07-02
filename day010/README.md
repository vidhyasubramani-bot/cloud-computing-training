# Kubernetes Deployment

## What is Deployment?

A **Deployment** is a Kubernetes resource that manages Pods and ensures the desired number of Pods are always running.

## Why do we use Deployment?

* Automatically creates Pods
* Recreates Pods if they fail
* Scales applications up or down
* Performs rolling updates
* Supports rollbacks

## Architecture

```text
Deployment
    │
    ▼
ReplicaSet
    │
    ▼
Pods
```

## Workflow

1. Create a Deployment.
2. Deployment creates a ReplicaSet.
3. ReplicaSet creates the required Pods.
4. If a Pod fails, ReplicaSet creates a new one automatically.
5. Deployment manages updates and scaling.

## Example Command

```bash
kubectl create deployment nginx --image=nginx --replicas=3
```

## Key Points

* Deployment manages ReplicaSets.
* ReplicaSet manages Pods.
* Pods run the application.
* Deployment provides self-healing, scaling, and rolling updates.

## Conclusion

Deployment is the recommended way to deploy and manage applications in Kubernetes because it automates Pod management, scaling, updates, and recovery.
