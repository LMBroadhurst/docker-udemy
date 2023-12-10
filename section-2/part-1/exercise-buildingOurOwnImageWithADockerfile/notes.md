# Dockerfile
- Look at the image that has been built and the notes surrounding them

## Building an image (or creating a container from that image)

```bash
docker build .
# => => writing image sha256:ff39a30d22bb7b6e3aaf1370576ed95c3a7a97187331ff71a384a7a250514a36

docker run ff39a30d22bb7b6e3aaf1370576ed95c3a7a97187331ff71a384a7a250514a36
# ... no response as the command 'doesn't finish'

# Can't access localhost 80 though
docker stop exciting_nobel

# -a shows all containers. Without -a shows all *running* containers
docker ps -a
# CONTAINER ID   IMAGE          COMMAND                  CREATED          STATUS                        PORTS     NAMES
# f448d1072a7d   ff39a30d22bb   "docker-entrypoint.s…"   3 minutes ago    Exited (137) 20 seconds ago             exciting_nobel

# Exposes port 80 via the local machines port 3000
docker run -p 3000:80 ff39a30d22bb
```