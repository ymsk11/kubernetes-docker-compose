# kubernetes-docker-compose

```
docker-compose up -d --force-recreate --build
kubectl config set-cluster localhost --insecure-skip-tls-verify=true --server=http://localhost:8888
kubectl config set-context localhost --cluster=localhost
kubectl config use-context localhost
kubectl get pods
```

now status
```
% kubectl get cs      
NAME                 STATUS      MESSAGE                                                                                        ERROR
scheduler            Unhealthy   Get http://127.0.0.1:10251/healthz: dial tcp 127.0.0.1:10251: getsockopt: connection refused
controller-manager   Unhealthy   Get http://127.0.0.1:10252/healthz: dial tcp 127.0.0.1:10252: getsockopt: connection refused
etcd-0               Healthy     {"health": "true"}
% kubectl get nodes   
NAME           STATUS    ROLES     AGE       VERSION
ef8e47864969   Ready     <none>    3m        v1.9.0
% kubectl get pods   
No resources found.
```
