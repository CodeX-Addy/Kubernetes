# To create the pods
kubectl run --image=nginx nginx-pod

# To get pods
kubectl get pods

# To check the logs for a pod
kubectl logs nginx-pod

# For real time logs
kubectl logs -f nginx-pod

# To describe the pods
kubectl describe pod nginx-pod  
kubectl describe pod/nginx-pod
