FROM ubuntu:latest

LABEL MANTAINER="Davide Garbezza"

USER root

RUN apt update && apt install -y redis-server

EXPOSE 6380/tcp

USER redis

COPY ./redis.conf  /etc/redis/ 

CMD redis-server /etc/redis/redis.conf


