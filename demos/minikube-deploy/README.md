# Minikube Deploy Demo

Installing Minikube and deploying an nginx service on a local Kubernetes cluster.

## Steps shown

```bash
brew install minikube
minikube version
minikube start
kubectl apply -f deployment.yaml
kubectl expose deployment nginx-deployment --type=NodePort --port=80
minikube service nginx-deployment --url
```

## Files

| File | Description |
|------|-------------|
| `mink.gif` | GIF recording of the full workflow |
| `deployment.yaml` | nginx deployment manifest used in the demo |
