# k8s-admin

## Setup k3s
```
curl -sLS https://get.k3sup.dev | sh
sudo install k3sup /usr/local/bin/

k3sup --help
```

```
export IP=192.168.1.200

k3sup install --ip $IP --user michal --k3s-extra-args '--disable=servicelb --disable=traefik'
```

```
export KUBECONFIG=`pwd`/kubeconfig
kubectl get node
```
