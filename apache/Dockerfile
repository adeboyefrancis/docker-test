# Use the Ubuntu base image
FROM ubuntu

LABEL maintainer="Francis Adeboye <adeboye.francis@icloud.com>"

# Install the Apache HTTP server package from the Ubuntu repository
RUN apt-get update && \
    apt-get install -y tzdata apache2 && \
    apt-get clean

# Copy the index.html file to the Apache document root
COPY index.html /var/www/html/

# Specify the command to run when the container starts
CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]

# Expose port 80 to allow incoming HTTP traffic to the container
EXPOSE 80