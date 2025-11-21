Now generate token:
```
kubectl create token jenkins -n webapps
```

This is the token you put in Jenkins Kubernetes plugin → Credentials (Secret Text).

Kubernetes can only apply raw YAML, so you must use the raw.githubusercontent.com URL.
```
kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/main/deploy/static/provider/cloud/deploy.yaml

```
Before you begin
You must use a kubectl version that is within one minor version difference of your cluster. For example, a v1.34 client can communicate with v1.33, v1.34, and v1.35 control planes. Using the latest compatible version of kubectl helps avoid unforeseen issues.
####
also create token in infra and save token to jenkins credentials again
