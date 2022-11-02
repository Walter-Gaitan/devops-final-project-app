# Github Workflow for building and testing the project

## ECR
When a push is done from a branch aside from main, the workflow will build the docker image and push it to the ECR repository.

## Tag
When a tag is pushed to the repository, the workflow will be triggered. The workflow will build the Docker image and push it to the ECR repository.