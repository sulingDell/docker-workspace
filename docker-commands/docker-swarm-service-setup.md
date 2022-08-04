# Deployment of docker container on docker swarm.

# Create docker swarm service -> ( Services are going to Host / Bind Containers )
- Pull docker images
- Create a docker service
- Verify the service & containers

---------------------------------------------------------

# PHP Application
- sudo docker pull wahid74/phpcode
- sudo docker service create -p 80:80 --name php-service wahid74/phpcode

# Verify list docker swarm service
> sudo docker service ls

# list container for service
> sudo docker ps -a

---------------------------------------------------------
# Spring boot application
- sudo docker pull wahid74/ecom-webservice
- sudo docker service create -p 8080:8081 --name ecom-service wahid74/ecom-webservice

# Verify list docker swarm service
> sudo docker service ls

# list container for service
> sudo docker ps -a


