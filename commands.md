### List all PODs
kubectl get pods

### Get POD Details
kubectl describe pod node-express-sample

### Exposing a POD through service
kubectl expose pod node-express-sample --type=LoadBalancer --port=8080 --target-port=4000

### list all services
kubectl get services

minikube tunnel

kubectl apply -f health-check.yaml

kubectl delete svc node-express-sample

