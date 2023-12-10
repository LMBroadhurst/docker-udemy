```bash
docker rm <'container-name'>
# Container must not be running to remove a container

# To show all docker images
docker images

docker rmi <'image'>
# Must remove containers belonging to images before deleting an image

docker image prune
# remove all unused images

# We can also remove a container automatically when exiting a container
# Can be very useful to stop cluttering of container space
# Useful when code changes come often
docker run -p 3000:80 --rm <'image'>
```

```bash
docker image inspect <'docker-id'>
```