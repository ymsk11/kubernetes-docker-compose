# kubernetes-docker-compose

```
docker-compose up -d --force-recreate --build
kubectl config set-cluster localhost --insecure-skip-tls-verify=true --server=http://localhost:8888
kubectl config set-context localhost --cluster=localhost
kubectl config use-context localhost
kubectl get pods
```
