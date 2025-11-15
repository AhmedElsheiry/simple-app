# My Kubernetes Project

This project contains a Deployment, Service, and Ingress for a simple NGINX app.

## Requirements
- Minikube
- kubectl
- Ingress addon enabled

## Run
```bash

kubectl apply -f namespace.yaml
kubectl apply -f secret.yaml
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
kubectl apply -f ingress.yaml

## Test the app on a browser
minikube ip
vi /etc/hosts
Add the ip with myapp.local
search http://myapp.local/ on your browser
