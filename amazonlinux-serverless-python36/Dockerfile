# amazonlinux with AWS CLI and serverless
FROM amazonlinux:2-with-sources

RUN yum update -y && \
    curl -o- -L https://slss.io/install | bash && \
    curl -sL https://dl.yarnpkg.com/rpm/yarn.repo -o /etc/yum.repos.d/yarn.repo && \
    curl -sL https://rpm.nodesource.com/setup_12.x | bash - && \
    curl -o- -L https://slss.io/install | bash && \
    yum install -y gcc-c++ make rsync nodejs12 yarn aws-cli unzip wget tar && \
    amazon-linux-extras install -y docker python3=3.6.2 && \
    yum clean all && rm -rf /var/cache/yum

