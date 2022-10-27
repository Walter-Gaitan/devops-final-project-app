# Application for EKS cluster

Prerequisites
- Docker
- ArgoCD
- AWS CLI
- Kubectl
- MongoDB Atlas Cluster

## Description

## Usage


To create the ECR repository, run the following command:

```bash
aws ecr create-repository --repository-name rest-api --image-scanning-configuration scanOnPush=true --image-tag-mutability IMMUTABLE --region us-east-1
```

## Github Actions
