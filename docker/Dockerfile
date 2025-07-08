FROM nginx:latest

RUN apt-get update && \
  apt-get install -y iputils-ping default-mysql-client && \
  rm -rf /var/lib/apt/lists/*

COPY files/index.html /usr/share/nginx/html/index.html
