kubectl apply -f deployment.yaml
kubectl describe <pod-name>
kubectl exec -it <pod-name> -c main-app -- sh -c 'echo $CONTAINER_TYPE'
kubectl exec -it <pod-name> -c sidecar -- sh -c 'echo $CONTAINER_TYPE'
kubectl get deployment
