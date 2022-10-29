FROM ubuntu:22.04

RUN apt update
RUN DEBIAN_FRONTEND=nointeractive apt install -y awscli
RUN DEBIAN_FRONTEND=nointeractive apt install -y python3-pip && \
    pip install ansible --upgrade