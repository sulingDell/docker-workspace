# create / run a container
> sudo docker run -it ubuntu /bin/bash

# ssh / login a container
> sudo docker exec -it <container-name> /bin/bash
> sudo docker exec -it ubuntu /bin/bash
> sudo docker exec -it bc498b019577 /bin/bash

# start container
> sudo docker container start <container-name>/<container-id>
> sudo docker container start bc498b019577
> sudo docker container start determined_hofstadter

# stop container
> sudo docker container stop <container-name>/<container-id>
> sudo docker container stop bc498b019577
> sudo docker container stop determined_hofstadter

# restart container
> sudo docker container restart <container-name>/<container-id>
> sudo docker container restart bc498b019577
> sudo docker container restart determined_hofstadter


# delete container (You cannot remove a running container : stop container can be deleted)
> sudo docker container rm <container-name>/<container-id>
> sudo docker container rm bc498b019577
> sudo docker container rm determined_hofstadter

# forcefull delete container ( delete a running container)
> sudo docker container rm -f <container-name>/<container-id>
> sudo docker container rm -f determined_hofstadter
> sudo docker container rm -f bc498b019577