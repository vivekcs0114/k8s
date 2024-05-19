## ingress setup

Configure Ingress rule for the different service available.

### Install ingress

```
helm upgrade --install ingress .
```

### Check the ingress config reflected correctly

Set up Ingress on Minikube with the NGINX Ingress Controller

minikube addons enable ingress

kubectl get pods -n ingress-nginx

minikube ip

/etc/hosts
<minikube ip>    k8s-app.test
