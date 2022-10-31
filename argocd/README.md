# Configure ArgoCD

1. Install ArgoCD. You can follow the instructions to install it [here](https://argoproj.github.io/argo-cd/getting_started/).
2. Create the application configuration file. This is already created, it is called ```application.yaml```.
Make sure to change the ```repoURL``` to your own repo.
3. Apply the configuration file using the following command:
```bash
kubectl apply -f application.yaml
```
4. Navigate to the ArgoCD UI. You will see that the application is deployed. ![ArgoCD UI](../images/argo.png)