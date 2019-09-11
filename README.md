# AKSHelloWorldHelmInit

AKS and Helm introduction presentation.

This repo contains a presentation [slide deck](slide_deck.pdf) and also samples used in the demo.

```
#Pod Information
kubectl get pods
kubectl describe pod <pod_name>

#Node Information
kubectl get nodes
kubectl describe node <node name>

#Deployment Information
kubectl get deployments
kubectl describe deployment <deployment name>

# Running and exposing a deployment manually
kubectl run hello --image=tutum/hello-world --port=80 --replicas=2
kubectl expose deployment hello --type=LoadBalancer --port=80 --target-port=80
kubectl scale deployment hello --replicas=3

# Getting access to a POD
kubectl exec -it <podname> /bin/bash    

#Installing via kubernetes yaml files
kubectl apply -f azurevote.yml
kybectl apply - azurevote2.yml

#Helm commands
helm install . --name azurevote3 --set title=HiHi,value1=vim,value2=emacs
helm upgrade  --set title=Wow,value1=Spacex,value2=Nasa azurevote4 .
```


