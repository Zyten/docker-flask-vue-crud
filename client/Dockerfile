FROM node:14-alpine

# make the 'app' folder the current working directory
WORKDIR /root/app/client

# copy both 'package.json' and 'package-lock.json' (if available)
COPY package*.json ./

# install project dependencies
RUN npm install
