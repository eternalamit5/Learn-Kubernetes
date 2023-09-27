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


# Kubernetes Service: 

- Kubernetes Service: Using service we can expose specific ports from deployment. It is way to connect to specific pods from outside Kubernetes node i.e; from external computer
- Service is like a virtual server. It has its own IP called as cluster IP of service.


![Screenshot from 2023-09-27 12-16-13](https://github.com/eternalamit5/Learn-Kubernetes/assets/44448083/143b7fa9-2e54-4681-ae50-c267df71a5ce)

![Screenshot from 2023-09-27 12-18-02](https://github.com/eternalamit5/Learn-Kubernetes/assets/44448083/3cbc70cf-40d8-4a77-ad40-76f9af803dff)


![Screenshot from 2023-09-27 12-23-29](https://github.com/eternalamit5/Learn-Kubernetes/assets/44448083/57e8e2db-f82a-4782-9f4e-3bc5f7f521ad)





There are 3 kinds of service:
1. Node port service
2. Cluster IP
3. Load Balancer

# Node port service

![Screenshot from 2023-09-27 12-21-56](https://github.com/eternalamit5/Learn-Kubernetes/assets/44448083/c6240212-e221-4b70-9601-5b6fdfc6de48)


![Screenshot from 2023-09-27 12-24-08](https://github.com/eternalamit5/Learn-Kubernetes/assets/44448083/74be2737-0060-417e-a83b-f88b8504b061)

![Screenshot from 2023-09-27 12-24-23](https://github.com/eternalamit5/Learn-Kubernetes/assets/44448083/6bbe3993-4318-49cc-ba6f-8f4365cb4bd5)

![Screenshot from 2023-09-27 12-26-04](https://github.com/eternalamit5/Learn-Kubernetes/assets/44448083/b52a69b0-c158-42f6-ad38-2bb53a9852c7)

![Screenshot from 2023-09-27 12-26-18](https://github.com/eternalamit5/Learn-Kubernetes/assets/44448083/1e65aec5-93e3-4015-8bd3-ebc4ce676c09)

![Screenshot from 2023-09-27 12-29-17](https://github.com/eternalamit5/Learn-Kubernetes/assets/44448083/58dd72a0-a369-4f02-bc53-ae8106f7e237)

# Cluster IP

![Screenshot from 2023-09-27 13-31-25](https://github.com/eternalamit5/Learn-Kubernetes/assets/44448083/cc0afba4-262e-4f74-9787-02164b59f2da)


# Load Balancer

- It is mostly used with cloud service.
- 
![Screenshot from 2023-09-27 13-36-08](https://github.com/eternalamit5/Learn-Kubernetes/assets/44448083/09091a2a-4f5b-453a-b2dd-d773c39a91fa)


To list services:
        k get services

        or

        k get svc
