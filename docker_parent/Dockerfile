FROM nginx:latest
RUN rm -rf /usr/share/nginx/html/*
RUN apt update && apt install wget -y
RUN wget -P /usr/share/nginx/html/ https://raw.githubusercontent.com/vitaliy026-00/docker-neb0/main/docker_parent/index.html

