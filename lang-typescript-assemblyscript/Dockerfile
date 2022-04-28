FROM ubuntu:latest

MAINTAINER Zim Kalinowski

ENV TZ=Europe/Warsaw
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

RUN apt-get update
RUN apt-get install -y nodejs npm

RUN mkdir project
RUN cd project && npm install --save @assemblyscript/loader
RUN cd project && npm install --save-dev assemblyscript
