FROM ubuntu:latest

MAINTAINER Zim Kalinowski

RUN apt-get update
RUN apt-get install -y wget

RUN wget https://github.com/tinygo-org/tinygo/releases/download/v0.22.0/tinygo_0.22.0_amd64.deb
RUN dpkg -i tinygo_0.22.0_amd64.deb

