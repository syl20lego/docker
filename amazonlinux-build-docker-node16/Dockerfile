# amazonlinux with AWS CLI and node js 12
FROM amazonlinux:2-with-sources

RUN yum update -y && \
    curl -sL https://dl.yarnpkg.com/rpm/yarn.repo -o /etc/yum.repos.d/yarn.repo && \
    curl -sL https://rpm.nodesource.com/setup_16.x | bash - && \
    curl -o- -L https://slss.io/install | bash && \
    yum install -y gcc-c++ make rsync nodejs16 yarn aws-cli tar git openssh-clients && \
    amazon-linux-extras install -y docker && \
    yum clean all && rm -rf /var/cache/yum

