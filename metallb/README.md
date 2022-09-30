1. Create namespace and metallb objects
```
kubectl apply -f https://raw.githubusercontent.com/metallb/metallb/v0.13.5/config/manifests/metallb-native.yaml
```

2. Create configmap for metallb
```
kubectl apply -f config.yaml
```