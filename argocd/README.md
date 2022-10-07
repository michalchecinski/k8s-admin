# Install ArgoCD on cluster

Go through the docs: https://argo-cd.readthedocs.io/en/stable/getting_started/

```
kubectl create namespace argocd
kubectl apply -n argocd -k argocd/installation
```

```
kubectl -n argocd get secret argocd-initial-admin-secret -o jsonpath="{.data.password}" | base64 -d; echo
```

```
argocd login 192.168.1.202
```

```
argocd account update-password
```
