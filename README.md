# Helm template to deploy an API rest with postgreSQL and a react client. 



## Starting minikube 🛠️
To run this helm-template you need to run the following minikube commands before
deploying the resources 

Start minikube 
```bash
minikube start 
```
Enable nginx controller ingress. 
```bash
minikube addons enable ingress 
```
Creating the resources related with cert-manager 
```bash
kubectl apply -f https://github.com/cert-manager/cert-manager/releases/download/v1.13.2/cert-manager.yaml
```

## Create the directory in minikube 🛠️
Connect through ssh to server  
```bash
minikube ssh
```
Create the directory to be used as volume
```bash
mkdir -p customize-location && exit 
```

## install the template 🛠️
Connect through ssh to server  
```bash
helm install template-name
```


## Made by: 💭
- [Santiago Hadad](https://github.com/shadad00)