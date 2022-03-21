FROM ubuntu:latest

MAINTAINER Zim Kalinowski

ENV TZ=Europe/Warsaw
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

RUN apt-get update
RUN apt-get install -y git
RUN apt-get install -y cmake
RUN apt-get install -y build-essential

RUN git clone https://github.com/wasmx/fizzy.git
RUN cd fizzy && mkdir build && cd build && cmake -DFIZZY_WASI=ON .. && cmake --build .
RUN cd fizzy && build/bin/fizzy-wasi ./test/smoketests/wasi/helloworld.wasm
