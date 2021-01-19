```yml
 kubectl create -f pod-definition.yml --namespace lab
```


```yml
kubectl create -f rc-definition.yml --namespace lab --validate=false
```

```yml
kubectl replace -f replicaset-definition.yml --namespace lab
```

```yml
kubectl scale --replicas=6 -f replicaset-definition.yml --namespace lab
```

```yml
kubectl scale --replicas=6 replicaset myapp-replicaset --namespace lab
```

```yml
kubectl get replicaset
```

```yml
kubectl delete replicaset myapp-replicaset
```

```yml
kubectl get all --namespace lab
```

```yml
kubectl get pods --namespace lab -o yaml
```

```yml
kubectl get pods --namespace lab -o json
```

```yml
kubectl get pods --namespace lab -o wide
```

```yml
kubectl create namespace dev
```

```yml
kubectl config set-context $(kubectl config current-context) --namespace=dev
```