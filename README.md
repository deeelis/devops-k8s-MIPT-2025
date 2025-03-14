# Hometasks K8S

Здесь собраны манифесты Kubernetes для Apache HTTP Server и Redis

## Deployment

1. Создайте namespace zaitseva-hw3

```
kubectl create namespace zaitseva-hw3
```

2. Примените манифесты для Apache HTTP Server

```
kubectl apply -f httpd-deployment.yaml
kubectl apply -f httpd-service.yaml
kubectl apply -f app-config.yaml
kubectl apply -f db-credentials.yaml
```

3. Примените манифесты для Redis

```
kubectl apply -f redis-config.yaml
kubectl apply -f redis-credentials.yaml
kubectl apply -f redis-deployment.yaml
kubectl apply -f redis-service.yaml
```
