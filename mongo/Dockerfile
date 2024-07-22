# Use the official MongoDB image from the Docker Hub
FROM mongo:4.4
# Create the MongoDB data directory
RUN mkdir -p /data/db
# Expose port #27017 from the container to the host
EXPOSE 27017
# Set /usr/bin/mongod as the dockerized entry-point application
CMD ["mongod"]