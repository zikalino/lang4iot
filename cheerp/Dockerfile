FROM ubuntu:latest

MAINTAINER Zim Kalinowski

RUN apt-get update
RUN apt-get install -y software-properties-common
RUN apt-get update
RUN add-apt-repository ppa:leaningtech-dev/cheerp-ppa
RUN apt-get install -y cheerp-llvm-clang=2.7~rc1-1~focal
RUN apt-get install -y cheerp-core
