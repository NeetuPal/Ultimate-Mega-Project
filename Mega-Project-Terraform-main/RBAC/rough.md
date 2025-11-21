Now generate token:
```
kubectl create token jenkins -n webapps
```

This is the token you put in Jenkins Kubernetes plugin → Credentials (Secret Text).

Kubernetes can only apply raw YAML, so you must use the raw.githubusercontent.com URL.
```
kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/main/deploy/static/provider/cloud/deploy.yaml

```
