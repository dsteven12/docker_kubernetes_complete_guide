# Specify a base image
FROM node:14-alpine

# Assign working directory to COPY files into. Can be usr, but can also be var or home
WORKDIR /usr/app

# COPY package.json file from local directory in docker directory
COPY ./package.json ./

# Install some dependencies
RUN npm install

# COPY remaining files from local directory into docker directory
# This allows cache to be used except when modifications are made to the package.json file.
COPY ./ ./

# Default Command
CMD ["npm", "start"]