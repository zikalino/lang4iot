FROM ubuntu:latest

MAINTAINER Zim Kalinowski


RUN apt-get update
RUN apt-get install -y git
RUN apt-get -y install python3 python3-pip

RUN git clone https://github.com/emscripten-core/emsdk.git
RUN cd emsdk && git pull

RUN cd emsdk && ./emsdk install latest
RUN cd emsdk && ./emsdk activate latest
RUN cd emsdk && chmod 777 ./emsdk_env.sh
RUN cd emsdk && /bin/bash -c ./emsdk_env.sh
