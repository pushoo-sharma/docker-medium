# build (pull the images it need mongo, node, etc) and once it is done we are able to run all the containers
docker-compose build

# make the container up and running
docker-compose up

# stop all three container
docker-compose stop


-- Pushpak Sharma

# the command to add a worker to the swarm
docker swarm init

# Notes : SSH into the machine that you want to add to the swarm and then once you're actually in the machine, you could basically run this command and it's going to add that machine to the swarm.

# Docker info like usual and it's going to give you all the information on your Docker install and all the containers and the swarms that you have installed. So if we look all the way up, you're seeing that we have four containers.

docker info

# And now we see that we have one manager that is this particular ID here, and this is the swarm.

docker node ls

# Adding nodes to the swarm
docker stack deploy -c docker-compose.yml

# Adding nodes to the swarm
docker service create --replicas 1 --name nodeserver2 node ping docker.com

# check the service u created
docker service ls

## Overview of 
kubectl version --client

# a cluster started or a new cluster created.
minikube start

# check for your cluster
kubectl cluster-info

# deployment
kubectl create deployment nodeapplication2 --image=node

# get the deployments
kubectl get deployments








