FROM node

WORKDIR /app

# First copy over the package.json and run npm install
# This means we do not have to rerun npm install every time we make a change to our application code
# Only when we make a change to the package.json file
# Previously is we made a change to the server file we would have to re-run npm install, wasting time
COPY package.json /app

RUN npm install

COPY . /app

# Expose port 80 to the local machine
# This is actually just documentation, it does not actually do anything, optional line
# Need to perform port mapping when running the container
EXPOSE 80

# Keep in mind this is an image, not a container.
# Therefore, we should not run the application here e.g. node server.js
# We need to use the CMD command to run the application when we create/start a container from this image.
# This should always be the last command in the Dockerfile.
CMD ["node", "server.js"]