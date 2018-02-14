# kubernetes-docker-compose

## start
```
% docker-compose up -d --force-recreate --build
% kubectl config set-cluster localhost --insecure-skip-tls-verify=true --server=http://localhost:8888
% kubectl config set-context localhost --cluster=localhost
% kubectl config use-context localhost
```

## deploy sample.yaml
```
% kubectl create -f sample.yaml
% kubectl get pods                                                                                                                                                  (git)-[master]
NAME        READY     STATUS    RESTARTS   AGE
nginx-pod   1/1       Running   0          2m
```
```
% kubectl get cs      
NAME                 STATUS      MESSAGE                                                                                        ERROR
scheduler            Unhealthy   Get http://127.0.0.1:10251/healthz: dial tcp 127.0.0.1:10251: getsockopt: connection refused
controller-manager   Unhealthy   Get http://127.0.0.1:10252/healthz: dial tcp 127.0.0.1:10252: getsockopt: connection refused
etcd-0               Healthy     {"health": "true"}
% kubectl get nodes   
NAME           STATUS    ROLES     AGE       VERSION
ef8e47864969   Ready     <none>    3m        v1.9.0
```
