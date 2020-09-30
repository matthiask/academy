#TODO: Describe each Line

# Base image: node:current-slim
FROM node:current-slim

# Work in /usr/src/app _inside_ the container
WORKDIR /usr/src/app

# Copy the local package.json into container:/usr/src/app
COPY package.json .

# Run npm install
RUN npm install

# Inform Docker that the container will listen on port 8080
EXPOSE 8080

# Run npm start
CMD [ "npm", "start" ]

# Copy the contents of this directory to container:/usr/src/app
COPY . .
