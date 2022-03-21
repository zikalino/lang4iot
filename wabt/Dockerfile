FROM ubuntu:latest

MAINTAINER Zim Kalinowski

ENV TZ=Europe/Warsaw
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

RUN apt-get update
RUN apt-get install -y git
RUN apt-get install -y cmake
RUN apt-get install -y build-essential

RUN git clone --recursive https://github.com/WebAssembly/wabt
RUN cd wabt && git submodule update --init
RUN cd wabt && mkdir build && cd build && cmake .. && cmake --build .
