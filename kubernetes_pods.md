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

# To generate the yaml
kubectl get pod nginx-pod -o yaml

# To create pods using yaml
kubectl create -f pod.yaml

# Generating yaml using dry run
kubectl run nginx-pod --image=nginx --dry-run=client -o yaml > pod1.yaml

# To edit the running pods
kubectl edit pod nginx-pod

# To check the labels
kubectl get pods --show-labels
