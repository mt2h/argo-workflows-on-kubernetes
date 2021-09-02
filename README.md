# Argo workflows on Kubernetes

## Install Argo

```bash
#https://argoproj.github.io/argo-workflows/quick-start/
kubectl create ns argo
kubectl apply -n argo -f https://raw.githubusercontent.com/argoproj/argo-workflows/master/manifests/quick-start-postgres.yaml
kubectl -n argo port-forward deployment/argo-server 2746:2746
https://localhost:2746/
```

## Commands Workflow

```bash
kubectl create -f wf-hello-world.yaml -n argo
kubectl get workflow -n argo
```
