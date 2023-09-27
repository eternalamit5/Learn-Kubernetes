# Learn Kubernetes 

## Important commands to get started

1. Start minikube cluster:

        minikube start --driver=virtualbox

2. To see the status of the minikube

        minikube status

        minikube ip

3. To ssh into the Kubernetes node:
        ssh docker@your IP address

   login: username is docker and password is tcuser (tcuser is not working check in stackoverflow)

   after that we are inside kubernetes node.

   
# Kubectl commands

1. To get info of the cluster:
   
        kubectl cluster-info


 2. Ger node status:
        kubectl get nodes

        kubectl get pods

To see the all the namespaces:

        kubectl get namespaces    

To alias kubectl command.

        alias k="kubectl"

Create deployment

        k create


Kubernetes Service: using service we can expose specific port from deployment.

There are 3 kinds of service:
1. Node port service
2. Cluster IP
3. Load Balancer

To list services:
        k get services

        or

        k get svc
