#  Node 10 with AWS CLI
FROM node:10-buster

ARG CLI_VERSION=1.16.304

RUN apt update && \
    apt-get install -y python python-pip rsync && \
    pip install --upgrade awscli==$CLI_VERSION

VOLUME /root/.aws

VOLUME /project

WORKDIR /project