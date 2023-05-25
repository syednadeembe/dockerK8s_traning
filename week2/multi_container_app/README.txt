###Create the backend image
docker build -t hello-server .

###tag and push to DTR
docker tag hello-server syednadeembe/k8s-demo:hello-server

###deploy the backend service 
kubectl apply -f backend_deployment.yaml

### test the back end server by hitting 5000 port from the backend container

### use the backend svc in the nginx.conf for the frontend server

### create config map that uses the nginx.conf
kubectl create configmap nginx-configmap --from-file=nginx.conf

### deploy frontend server
k apply -f frontend_deployment.yaml

### check the svc and use the node port to login to the frontend server which internally will point to backend