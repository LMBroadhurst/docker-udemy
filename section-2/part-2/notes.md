# Managing Images & Containers
- All commands have a --help flag to see options

## Core commands

## 'Deprecated'

## Managing images and containers

```bash
docker ps
# All running containers

docker ps -a
# All containers (running and not running)

docker run
# Creates a new container based on an image
# By default it will start in attached mode

docker run -d
# Creates and starts container, in detached mode

docker start <'docker-container-name'>
# Starts a non running container
# This does not leave us 'inside' the docker environment
# The default mode for start is 'not attached'

docker ps
# Can now see the container is running

# Now we can connect to the container
docker attach <'docker-container-name'>

# Attached simply means the terminal is connected to the container and will print logs from node etc
# If not attached, the container port will still be exposed, can still vist the website, etc
```