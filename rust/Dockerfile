FROM ubuntu:latest

MAINTAINER Zim Kalinowski

ENV TZ=Europe/Warsaw
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

RUN apt-get update
RUN apt-get install -y curl
RUN curl https://sh.rustup.rs -sSf | sh -s -- --default-toolchain stable -y
ENV PATH=/root/.cargo/bin:$PATH

RUN rustup toolchain install nightly
RUN rustup update
RUN rustup target add wasm32-unknown-unknown --toolchain nightly
