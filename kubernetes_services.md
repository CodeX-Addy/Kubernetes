# Cluster IP

## To create a service
kubectl expose deploy nginx-deploy --port=80

## To get the svc
kubectl get svc

## To access the svc with url
minikube service nginx-deploy --url

## To check the endpoints
kubectl get ep
