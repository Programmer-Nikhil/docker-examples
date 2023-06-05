# docker-examples

# docker commands

# build

# 1. docker build -t <image-name>:<version-number>

# To check the docker container available

# 2. docker container ls [To check how many containers are there]

# To run the docker container with image

# 3. docker container run -d(detach) -p(port) 3000(host machine port):3000(docker port) <image-name>:<version-number>

# how to stop the running docker container

# 4. docker container stop <container-id>

# ignore file for docker can be created with .dockerignore

# List all the docker images

# 5. docker image ls

# -rm command will remove the previous container with same name and will allow you to reuse the same name again and again for docker image.

# 6. docker run -rm -d -p 5500:5500 --name <container-name> <image-name>

# To stop running docker image

# 7. docker stop <container-id>

# To check containers id, It also list all the running containers

# 8. docker ps

# how to assign/map current directory with docker directory

# 9. docker run --rm -d -p 5500:5500 -v ${pwd}:/app --name <container-name> <docker-image-name>

# To check the docker image logs

# 10. docker logs <docker-container-id>

# To go inside the docker container

# 11.1> docker exec -it <docker-container-id> bash(shell type)

# 11.2> ls

# 11.3> exit (to get out of the container folder)

# How to provide environment vailables to the docker

# 12. docker run --rm -d -p 5500:5500 -v ${pwd}:/app --env-file ./<env-file-path> --name <docker-container-name> <docker-image-name>
