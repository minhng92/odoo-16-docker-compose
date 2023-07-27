# VERSION 1.0
# AUTHOR: Phil Chen
# DOCKER HUB: https://hub.docker.com/u/nethacker
# DESCRIPTION: NGINX on Ubuntu 18.04
# SOURCE: https://github.com/nethacker/ubuntu-flask-gunicorn-nginx-docker-compose
FROM nginx
RUN apt-get update && apt-get install -y \
    build-essential \
    curl \
  && rm -rf /var/lib/apt/lists/*
COPY nginx.conf /etc/nginx/nginx.conf
COPY certs/ /etc/nginx/certs
CMD ["nginx", "-g", "daemon off;"]