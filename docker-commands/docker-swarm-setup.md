# Create a docker swarm cluster ( one manger and two worker )
- Create ec2 instance - Manager - Install docker (docker engine)
- Create ec2 instance - Worker  - Install docker (docker engine)
- Create ec2 instance - Worker  - Install docker (docker engine)

# Create a manager node as e2 instance.
- 1. create ec2 instance
- 2. connect ec2 instance 
- 3. install docker

# Create a worker node as e2 instance.
- 1. create ec2 instance
- 2. connect ec2 instance 
- 3. install docker

# Initialize a docker cluster ( manager node ) 
- sudo docker swarm init             // Swarm initialized: current node is a manager node.

# Verify nodes in cluster 
> sudo docker node ls

# To add a worker to swarm manager , run the following command:
- sudo docker swarm join --token SWMTKN-1-2br9amas6eyum0yq3t39ax84ohgz8cx3m46hofk1y2w600wthw-djsnemnut6d8e5dqnl9bq69zx 172.31.17.113:2377


# To add a manager to this swarm, run 
- sudo docker swarm join-token manager    // and follow the instructions.


# list docker swarm service 
- sudo docker service ls

# list  container for service
- sudo docker ps -a

