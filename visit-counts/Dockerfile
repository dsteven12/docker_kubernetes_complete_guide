# Base Image
FROM node:alpine

# Assign working directory
WORKDIR /usr/app

# Install dependencies
COPY ./package.json ./
RUN npm install 
COPY ./ ./

# Command 
CMD ["npm", "start"]