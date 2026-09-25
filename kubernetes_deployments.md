# To create a deployment
kubectl create deploy nginx-deploy --image=nginx --replicas=3

# Experimenting to delete a pod
kubectl delete pod nginx-deploy-4jkf43j  
kubectl get pods -> it will again returns 3 running pods 

# To check the deployments
kubectl get deploy

# To scale out the replicas
kubectl scale deployment nginx-deploy --replicas=2

# Checking the description of deployment 
kubectl describe deploy nginx-deploy 

# To create yaml 
kubectl create deploy sample --image=nginx --dry-run=client -o yaml > deploy.yaml
