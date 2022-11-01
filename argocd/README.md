# Configure ArgoCD

1. Install ArgoCD. You can follow the instructions to install it [here](https://argoproj.github.io/argo-cd/getting_started/).
2. Create the application configuration file. This is already created, it is called ```application.yaml```.
Make sure to change the ```repoURL``` to your own repo.
3. Apply the configuration file using the following command in the root folder:
```bash
kubectl apply -f argocd
```
4. Port forward the ArgoCD server using the following command:
```bash
kubectl port-forward svc/argocd-server -n argocd 8080:443
```
5. Navigate to http://localhost:8080 in your web browser and login using the following credentials:
```bash
username: admin
password: $(kubectl get secret argocd-initial-admin-secret -n argocd -o jsonpath="{.data.password}" | base64 -d)
```
You will see that the application is deployed. ![ArgoCD UI](../images/argo.png)
5. Navigate to the application URL. You will see the application running. ![Application](../images/app.png)