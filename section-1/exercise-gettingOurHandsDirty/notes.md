1. Need to create an image...
- This is done by creating a `Dockerfile`

My Dockerfile looks like this:

```bash
FROM node:14

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

EXPOSE 3000

CMD [ "node", "index.js" ]
```

2. Build the image...

In the Dockerfile folder:

```bash
docker build .
```

3. Run the image...

```bash
# The -p 3000:3000 flag is publishing the port 3000 of the docker image to port 3000 of the local machine
docker run -p 3000:3000 18951b12419e231bc375a278b454b84e27a67dab90c298e51509f1d59a7a05b0
```