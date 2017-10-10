FROM ubuntu

COPY docker-rust-entrypoint /

ENTRYPOINT /docker-rust-entrypoint

WORKDIR /application

RUN apt-get update -y

RUN apt-get install -y cargo curl rustc vim

