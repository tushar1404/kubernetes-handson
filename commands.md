### List all PODs
kubectl get pods

### Get POD Details
kubectl describe pod node-express-sample

### Exposing a POD through service
kubectl expose pod node-express-sample --type=LoadBalancer --port=8080 --target-port=4000

## expose load balancer services
minikube tunnel

### list all services
kubectl get services

## ingest health check manifest
kubectl apply -f health-check.yaml

### Delete Service
kubectl delete svc node-express-sample


## ingest deployment manifest
kubectl apply -f deployment.yaml

### Expose Deployment through service
kubectl expose deployment node-express-sample --type=LoadBalancer --port=8080 --target-port=4000


### Delete Service
kubectl delete svc node-express-sample

