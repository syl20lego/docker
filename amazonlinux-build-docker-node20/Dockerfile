# amazonlinux 2022 with AWS CLI and node js 20
FROM amazonlinux:2022-with-sources

RUN yum update -y && \
    yum install -y aws-cli tar docker git gcc-c++ make && \
    curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.5/install.sh | bash && \
    . ~/.nvm/nvm.sh && \
    nvm install 20.3.1 && \
    npm install --global yarn node-gyp && \
    npm install -g serverless && \
    yum clean all && rm -rf /var/cache/yum
ENV PATH "/root/.nvm/versions/node/20.3.1/bin:${PATH}"

