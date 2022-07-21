# Prerequisite : Java & Maven
- sudo apt install default-jdk -y
- sudo apt install maven -y

# step 1: Create a docker file
- git clone https://github.com/wahidKhan74/ecom-webservice.git
- docker file is available in ecom-webservice

# step 2: Docker build image
- sudo docker build -t ecom-webservice -f Dockerfile / filepath
- sudo docker build -t ecom-webservice .

# step 3: Verify build images
- sudo docker images

# step 4: start / run container from custom docker image
- sudo docker run --name ecom-server -p 8080:8081 -d ecom-webservice