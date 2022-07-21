# Host website within ubuntu image based container

- sudo docker run --name webserver -p 80:80 -it ubuntu /bin/bash

  # Host website we need server
  - apt update
  - apt install apache2 -y
  - service apache2 status
  - service apache2 start
  - service apache2 stop
  - service apache2 restart
  - apt install git -y
  - git clone https://github.com/wahidKhan74/circus-website.git
  - cp -r circus-website/* /var/www/html/ 

# start container
- sudo docker container start a1231a120e04

# login container
- sudo docker exec -it a1231a120e04 /bin/bash
   - service apache2 restart