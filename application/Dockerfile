# FROM ubuntu:latest

# ENV UBUNTU_HOME=/var/www/html/
# RUN apt-get update -y
# ENV DEBIAN_FRONTEND noninteractive	
# RUN apt-get -y install tzdata
# RUN apt-get install apache2 -y
# WORKDIR UBUNTU_HOME
# COPY application/scripts/index.html ${UBUNTU_HOME}
# EXPOSE 80
# CMD ["apachectl" , "-D","FOREGROUND"]


# Use the official Nginx base image
FROM bitnami/nginx:1.14.0

# Copy the custom index.html to the default Nginx web root directory
COPY application/scripts/index.html /usr/share/nginx/html/

# Expose port 80 to the outside world
EXPOSE 80