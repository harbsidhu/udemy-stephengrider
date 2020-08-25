# Specify a base image

# FROM alpine # the base alpine image does not have npm installed, so will error
FROM node:alpine

# WORKDIR creates a working directory and copies all modules and files in this dir instead of root
WORKDIR /usr/simpleweb

# Install dependencies
# COPY copies required files package.json & indes,js into the container 

COPY ./package.json ./     
RUN npm install

# Will build using the code changes only
COPY ./ ./

# Command to run at container startup

CMD ["npm", "start"]
