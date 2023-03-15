#Sets up a container base on the alpine version of Node.js v18
FROM node:16-alpine
#Creates a working directory within the container
WORKDIR /usr/src/app
#Copies the 'package.json' and 'package-lock.json files into it
COPY package*.json ./
#Runs this command
RUN npm install
#Copies the remaining files in the project directory to the container's working directory
COPY . .
#Exposes the port 8080 to the host machine
EXPOSE 8080
#Specifies the command to be executed when the container starts
CMD [ "npm", "run", "serve"]


