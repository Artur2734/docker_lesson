
#docker network create MyNetwork


# Use Ubuntu as the base image
FROM ubuntu

# Install Nginx
RUN apt-get update && \
    apt-get install -y nginx && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

# Expose port 8080
EXPOSE 8080

# Start Nginx in the foreground
CMD ["nginx", "-g", "daemon off;"]


#docker build -t nginx_custom

#docker run -d --name nginx_container --network MyNetwork -p 8080:8080 nginx_custom
#docker run -it --name ubuntu_container --network MyNetwork ubuntu
#curl nginx_container:8080git 