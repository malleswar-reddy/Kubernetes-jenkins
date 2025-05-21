# Kubernetes-jenkins
Kubernetes-jenkins


# If you're using Jenkins with Minikube locally:

    . Add minikube image load to your Jenkinsfile after the Docker build step:

```shell

sh 'docker build -t my-spring-app:latest .'
sh 'minikube image load my-spring-app:latest'

```

# Call APi 

```url

curl http://spring.local:8081/api/hello

```
## Check Logs to Confirm App is Running
```shell

kubectl logs deployment/spring-app

```

# chek pod status
```shell
kubectl describe pod spring-app-<pod-id>
```

# Check the status of the pods
```shell
kubectl get pods
```
# Check the status of the services
```shell
kubectl get services
```
# Check the status of the deployments
```shell    
kubectl get deployments
```

# Check the stop
```shell
kubectl delete all --all --all-namespaces

