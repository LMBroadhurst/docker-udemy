# Covers 2 fundamental concepts, Images & Containers

## Images
- How they are related to containers
- Need images and containers to work with docker
- Using pre-built and custom images
- Create and manage containers

## Containers
- Small packages that is a 'unit of software'
- Run containers that are based on images
- "Running instance of an image"

## Images
- Templates/Blueprints for containers
- Contains code + required tools/runtimes
- An image can be used to create many containers (cattle)

## Where can we find images?
- Use existing pre-built image. Great source for this is 'dockerhub'
- Here can find images such as an official node.js image

```bash
# Creates a container on our local machine, from dockerhub since we had no local 'node' image
docker run node

# Will start a node docker environment we can work in
docker run -it node

# GPT -- -it flag
# The -it flags are commonly used together in Docker to allocate an interactive terminal within the container. Here's what each flag does:
# The -i flag stands for "interactive" and allows you to interact with the container by providing an open stdin.
# The -t flag allocates a pseudo-TTY (terminal).
```

## Creating custom images
- Can also write our own images using a Dockerfile
- Or build upon an existing image