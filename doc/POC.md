## How to login to argocd

https://34.118.24.94:8089

## If you have access to cluster then you should change admin password

```
kubectl config set-context --current --namespace=argocd
argocd admin initial-password -n argocd
argocd account update-password --account admin
```