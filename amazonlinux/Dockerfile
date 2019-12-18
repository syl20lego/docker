# amazonlinux with AWS CLI and node js 10
FROM amazonlinux:2

RUN curl -sL https://dl.yarnpkg.com/rpm/yarn.repo -o /etc/yum.repos.d/yarn.repo && \
    curl -sL https://rpm.nodesource.com/setup_10.x | bash - && \
    yum install -y gcc-c++ make rsync nodejs10 yarn aws-cli

VOLUME /project

WORKDIR /project
