# amazonlinux with AWS CLI and node js 10
FROM amazonlinux:2-with-sources

RUN yum update -y && \
    curl -sL https://dl.yarnpkg.com/rpm/yarn.repo -o /etc/yum.repos.d/yarn.repo && \
    curl -sL https://rpm.nodesource.com/setup_10.x | bash - && \
    yum install -y gcc-c++ make rsync nodejs10 yarn aws-cli  && \
    amazon-linux-extras install -y docker && \
    yum clean all && rm -rf /var/cache/yum

