# docker-with-node-react

## Commands


### Pull docker image
`docker pull <image_name>` <br />
Example: `docker pull node`

### Build a docker image from dockerfile
`docker build -t <docker_image_tag> .`<br />
Example: `docker build -t myapp .`

### list of docker images
`docker images` 

### Run docker image on a specific port
`docker run --name <docker_container_name> -p port:port <docker_image>`<br />
Example: `docker run --name myapp1_c -p 4000:4000 myapp`

### Run docker image on a specific port on detached mode
`docker run --name <docker_container_name> -p port:port -d <docker_image>` <br />
Example: `docker run --name myapp1_c -p 4000:4000 -d myapp`

### Stop docker container
`docker stop <container_name>` <br />
Example: `docker stop myapp1_c`

### List of running docker containers
`docker ps`

### List of running and stopped all containers
`docker ps -a`

### Restart docker containers
`docker start <image_name>` <br />
Example: `docker start myapp1_c`

### Delete Docker image
`docker image rm <image_name>`

### Forcefully delete docker image
`docker image rm <image_name> -f`

### Delete docker container
`docker container rm <docker_container_name>`

### Remove all docker images, containers, volumes and caches
`docker system prune -a`

### Remove the container when stop
`docker run --name <container_name> -p port:port --rm <image_name>` <br />
Example: `docker run --name myapp_c -p 4000:4000 --rm myapp`

### Volume mapping in docker
`docker run --name <container_name> -p port:port --rm -v <local_project_directory>:<container_directory> -v <container_directory_node_modules> <image_name>` <br />
Example: `docker run --name myapp_c -p 4000:4000 --rm -v /Users/arafath1019/Desktop/Github/docker-with-node-react/api:/app -v /app/node_modules myapp`

### Up docker compose
`docker-compose up`

### Down docker compose
`docker-compose down`