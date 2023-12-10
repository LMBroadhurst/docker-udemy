FROM node

WORKDIR /app

COPY . /app

RUN npm install

# Expose port 80 to the local machine
# This is actually just documentation, it does not actually do anything, optional line
# Need to perform port mapping when running the container
EXPOSE 80

# Keep in mind this is an image, not a container.
# Therefore, we should not run the application here e.g. node server.js
# We need to use the CMD command to run the application when we create/start a container from this image.
# This should always be the last command in the Dockerfile.
CMD ["node", "server.js"]