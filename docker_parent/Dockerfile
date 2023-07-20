FROM nginx:latest
RUN rm -rf /usr/share/nginx/html/*
RUN rm -rf /etc/nginx/nginx.conf
COPY ./nginx.conf /etc/nginx/
RUN mkdir /etc/nginx/sites-available /etc/nginx/sites-enabled
COPY ./default.conf /etc/nginx/sites-available/
RUN ln -s /etc/nginx/sites-available/default.conf /etc/nginx/sites-enabled
RUN apt update && apt install wget -y
RUN wget -P /usr/share/nginx/html/ https://raw.githubusercontent.com/vitaliy026-00/docker-neb0/main/docker_parent/index.html
COPY ./11.txt ./22.txt /usr/share/nginx/html/docs/
