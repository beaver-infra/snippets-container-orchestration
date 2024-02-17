# Snippets Container Orchestration

## Env Setup

Setup Postgres
```console
kubectl create secret generic pgpassword --from-literal PGPASSWORD=postgres
kubectl apply -f k8s_postgres
```

Setup Redis
```console
kubectl apply -f k8s_redis
```

Setup Py REST API v1.1.5 (docker image)
```console
kubectl apply -f k8s_pyrest
```

### Diagram

![Implementation Example](diagrams/k8s_setup.drawio.png)

### K8s Terms

**Ingress**

Deploy ingress-nginx controller
```console
kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/controller-v1.8.2/deploy/static/provider/cloud/deploy.yaml
minikube addons enable ingress
```

```
kubectl apply -f k8s-ingress.yaml
kubectl get ingress
```
