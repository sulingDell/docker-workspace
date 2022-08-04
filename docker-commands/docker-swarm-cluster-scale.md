# Create docker swarm service  - PHP Application
- sudo docker service create -p 80:80 --name php-service wahid74/phpcode

# Scaling up docker container on docker swarm
- Scale Up service -> increase replica container
- sudo docker service scale php-service=5

# Verify list docker swarm service
- sudo docker service ls

# list container for service
- sudo docker ps -a

# Scaling down docker container on docker swarm
- Scale down service -> decrease replica container
- sudo docker service scale php-service=3

# Verify list docker swarm service
- sudo docker service ls

# list container for service
- sudo docker ps -a

------------------------------------------------------------

# Create docker swarm service  - Spring boot Application
- sudo docker service create -p 8080:8081 --name ecom-service wahid74/ecom-webservice

# Scaling up docker container on docker swarm
- Scale Up service -> increase replica container
- sudo docker service scale ecom-service=5

# Verify list docker swarm service
- sudo docker service ls

# list container for service
- sudo docker ps -a

# Scaling down docker container on docker swarm
- Scale down service -> decrease replica container
- sudo docker service scale ecom-service=3

# Verify list docker swarm service
- sudo docker service ls

# list container for service
- sudo docker ps -a