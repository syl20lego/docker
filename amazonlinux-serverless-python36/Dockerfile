# amazonlinux with AWS CLI and serverless
FROM amazonlinux:2-with-sources

RUN yum update -y && \
    curl -o- -L https://slss.io/install | bash && \
    yum install -y aws-cli unzip wget && \
    amazon-linux-extras install -y python3=3.6.2 && \
    yum clean all && rm -rf /var/cache/yum

