# amazonlinux 2022 with AWS CLI and node js 18
FROM amazonlinux:2022-with-sources

RUN yum update -y && \
    yum install -y aws-cli tar docker && \
    curl -o- -L https://slss.io/install | bash && \
    curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.34.0/install.sh | bash && \
    . ~/.nvm/nvm.sh && \
    nvm install 18.12.1 && \
    npm install --global yarn && \
    yum clean all && rm -rf /var/cache/yum
ENV PATH "/root/.nvm/versions/node/v18.12.1/bin:${PATH}"

