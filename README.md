# DevOps Masterclass Examples

This repository contains sample Docker and Kubernetes files for the hello apps and tax calculator apps.

## Structure

- `docker/app1-hello`: Hello apps in Node, Python, and Spring Boot.
- `docker/app2-tax-calculator`: Tax calculator services and frontend examples.
- `k8s/aws/app1-hello/app.yaml`: AWS Kubernetes manifests for the hello apps.
- `k8s/aws/app2-tax-calculator`: Placeholder for tax calculator AWS manifests.
- `k8s/local`: Placeholder for local Kubernetes manifests.

## Apply App 1 Manifests

```bash
kubectl apply -f k8s/aws/app1-hello/app.yaml
kubectl get services -n app1-hello
```

Update the image names in `k8s/aws/app1-hello/app.yaml` before deploying to a remote cluster if your images are pushed under a Docker Hub username or another registry.
