FROM nginx:latest

RUN apt-get update && \
  apt-get install -y iputils-ping && \
  rm -rf /var/lib/apt/lists/*

COPY files/index.html /usr/share/nginx/html/index.html
