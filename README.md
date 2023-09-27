# Learn Kubernetes 

## Important commands to get started

1. Start minikube cluster:

      minikube start --driver=virtualbox

2. To see the status of the minikube

      minikube status

1. Bring the stack up:

        sudo docker compose -f docker-compose-test2.yml --env-file conf/variables.env up --pull always
