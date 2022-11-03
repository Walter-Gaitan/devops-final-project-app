# Kubernetes manifests

This directory contains Kubernetes manifests for deploying the application.


### Manifest
It creates the deployment and service for the application. Be sure to change the image URI to your own in line 21.
```yaml
    spec:
      containers:
      - image: 596027898727.dkr.ecr.us-east-1.amazonaws.com/mern-stack:0c5d849ba3fae1ae975de5b65f6053ca2e88f009
```

### Deployment
```bash
kubectl apply -f k8s
```