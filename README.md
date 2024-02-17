# Snippets Container Orchestration

```console
kubectl apply -f k8s_postgres
```
### Deployment

1. replicas
2. selector
3. template

### Service

1. type: NodePort / ClusterIP

### Persistent Volume Claim

1. accessmodes
2. resources > requests > storage


## Secrets

```console
kubectl create secret generic pgpassword --from-literal PGPASSWORD=postgres
```

```console
kubectl apply -f k8s_postgres
```