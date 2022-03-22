FROM ubuntu:latest

MAINTAINER Zim Kalinowski

RUN apt-get update
RUN apt-get install -y wget

RUN wget -c https://dl.google.com/go/go1.17.1.linux-amd64.tar.gz -O - | tar -xz -C /usr/local
RUN wget https://github.com/tinygo-org/tinygo/releases/download/v0.22.0/tinygo_0.22.0_amd64.deb
RUN dpkg -i tinygo_0.22.0_amd64.deb
ENV GOROOT=/usr/local/go

