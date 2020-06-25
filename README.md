# MINIKUBE COMMAND

## Basic Start
```
minikube start
```

## Check version
```
minikube version
```

## Start with hyperkit vm
```
minikube start --driver=hyperkit
```

## Enable addon
```
minikube addons enable ingress
```

## Enable Permission
```
sudo chmod 700 /Users/ChotipatP/.minikube/bin/docker-machine-driver-hyperkit 
```

## Start with multiple node 
https://minikube.sigs.k8s.io/docs/tutorials/multi_node/
```
minikube start --nodes 2 -p multinode-demo
```

## Dashboard
```
minikube dashboard
```

## Get Service url
```
minikube service <your_servicename> -n <your_namespace>
```

## Clear minikube
```
minikube stop
minikube delete
rm -rf ~/.minikube
```

# K8S COMMAND

## Check version
```
kubectl version --client
```

## Deployment
apply equal upsert
-f equal file -k equal folder
```
kubectl apply -f deployment.yaml
```

## Get node
```
kubectl get nodes
```

## Get service
```
kubectl get services
```

## Select namespace
```
kubectl config set-context --current --namespace=<your_namespace>
```

## Get all pod 
https://kubernetes.io/docs/concepts/workloads/controllers/deployment/
```
kubectl get pods --all-namespaces 
```

## Restart pod
```
kubectl -n <your_namespace> rollout restart deployment <your_namespace>
```

## Get pod in name space
```
kubectl get pods --namespace=<your_namespace>
```

## Get Ingress
https://kubernetes.io/docs/tasks/access-application-cluster/ingress-minikube/
```
kubectl get ingress
```

## Clear k8s
```
kubectl delete deployment <your_deploymentname>
kubectl delete service <your_servicename>
```
