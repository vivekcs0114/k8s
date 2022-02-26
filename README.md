# k8s setup

## Prerequisite
1. docker
2. kubectl
3. helm
4. minikube

### Installation Guid : -
1. follow this to install docker 
https://docs.docker.com/engine/install/ubuntu/

2. follow this to install kubectl
https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/

3. follow this to install helm
https://helm.sh/docs/intro/install/

4. follow this to install minikube on your m/c
https://minikube.sigs.k8s.io/docs/start/

### Once setup done, install all the helm chart one by one in the follwing sequence - 

1. Install ingress
```
helm upgrade --install ingress ./ingress
```

2. Install ping
```
helm upgrade --install ping ./ping
```
codebase - https://github.com/vivekcs0114/ping


3. Install pong
```
helm upgrade --install pong ./pong
```
codebase - https://github.com/vivekcs0114/pong


### To uninstall any one of the service 
```
helm uninstall {service-name}
```
e.g if you want to uninstall ping, 
```helm uninstall ping```

## Check if all the services are up and running
1. you can check k9s,  run this command from terminal  ```k9s```
2. you can check from the minikube dashboard, run this command from terminal  
```minikube dashboard```