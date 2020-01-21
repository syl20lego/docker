# docker
List of custom docker images

+ amazonlinux-node 10:
  AWS amzonelinux image node JS 10 for Fargate
  [syl20lego/amazonlinux-node10:1](https://hub.docker.com/repository/docker/syl20lego/amazonlinux-node/general])

+ amazonlinux-node 12:
  AWS amzonelinux image node JS 12 for Fargate
  [syl20lego/amazonlinux-node12:1](https://hub.docker.com/repository/docker/syl20lego/amazonlinux-node/general])


+ amazonlinux-build-awscli-node:
  AWS amzonelinux image with AWS CLI tools node JS 10 with yarn to build AWS lambda
  [syl20lego/amazonlinux-build-lambda10:1](https://hub.docker.com/repository/docker/syl20lego/amazonlinux-build-lambda/general])

+ amazonlinux-build-docker-node:
  AWS amzonelinux image with AWS CLI tools node JS 10 with yarn and docker, e.g. to build Fargate images
  [syl20lego/amazon-linux-build-docker10:2](https://hub.docker.com/repository/docker/syl20lego/amazonlinux-build-docker/general])

# Deploy

```
docker login
```

Build:

```
docker build --rm --no-cache -t image-amazonlinux-build-docker-node10 ./amazonlinux-build-docker-node10/
docker run -it image-amazonlinux-build-docker-node10 /bin/bash 
```

Publish:

```
docker tag image-amazonlinux-build-docker-node10 syl20lego/amazonlinux-build-docker-node10:3
docker push syl20lego/amazonlinux-build-docker-node10:3
```

Build:

```
docker build --rm --no-cache -t image-amazonlinux-build-docker-node12 ./amazonlinux-build-docker-node12/
docker run -it image-amazonlinux-build-docker-node12 /bin/bash 
```
Publish:

```
docker tag image-amazonlinux-build-docker-node12 syl20lego/amazonlinux-build-docker-node12:2
docker push syl20lego/amazonlinux-build-docker-node12:2
```

Build:

```
docker build --rm --no-cache  -t image-amazonlinux-build-awscli-node ./amazonlinux-build-awscli-node/
docker run -it image-amazonlinux-build-awscli-node /bin/bash 
```
Publish:

```
docker tag image-amazonlinux-build-awscli-node syl20lego/amazonlinux-build-awscli-node10:1
docker push syl20lego/amazonlinux-build-awscli-node10:1
```

Build:

```
docker build --rm --no-cache  -t image-amazonlinux-node ./amazonlinux-node/
docker run -it image-amazonlinux-node /bin/bash 
```
Publish:

```
docker tag image-amazonlinux-node syl20lego/amazonlinux-node10:1
docker push syl20lego/amazonlinux-node10:1
```

Build:

```
docker build --rm --no-cache  -t image-amazonlinux-serverless ./amazonlinux-serverless/
docker run -it image-amazonlinux-serverless /bin/bash 
```
Publish:

```
docker tag image-amazonlinux-serverless syl20lego/image-amazonlinux-serverless:1
docker push syl20lego/image-amazonlinux-serverless:1
```
