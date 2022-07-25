FROM ubuntu:xenial

MAINTAINER Zim Kalinowski

RUN apt-get update
RUN apt-get install -y software-properties-common
RUN apt-get update
RUN add-apt-repository ppa:leaningtech-dev/cheerp-ppa
RUN apt-get update
RUN apt-get install -y cheerp-llvm-clang
RUN apt-get install -y cheerp-core
