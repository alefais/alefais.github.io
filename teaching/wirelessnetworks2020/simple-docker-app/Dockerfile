# Specify a base image
FROM ubuntu:latest 

# Set the author of the new image
MAINTAINER Alessandra Faisalessandra.fais@phd.unipi.it

# Specify a working directory
WORKDIR /usr/app

# Install needed packages
RUN apt-get update && apt-get install -y cowsay fortune

# Copy entrypoint script file
COPY ./entrypoint.sh ./

# Give execute permission
RUN chmod +x entrypoint.sh

# Configure the container in order to run as an executable
ENTRYPOINT ["/usr/app/entrypoint.sh"]