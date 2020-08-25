# Use existing docker image for base

FROM alpine

# Change order of instructions
RUN apk add --update gcc 

# Download and install dependencies
RUN apk add --update redis

# Adding another run command,
# Build will used cache created previously 
#RUN apk add --update gcc 

# Tell image what to do at container startup
CMD ["redis-server"]
