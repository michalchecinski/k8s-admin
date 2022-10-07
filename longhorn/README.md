# Longhorn installation

After longhorn is installed via ArgoCD, run this command to delete default storage class from local:

```
kubectl patch storageclass local-path -p '{"metadata": {"annotations":{"storageclass.kubernetes.io/is-default-class":"false"}}}'
```