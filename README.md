# docker

```
docker login
```

## List of custom docker images

+ amazonlinux-node 10:
  AWS amzonelinux image node JS 10 for Fargate
  [syl20lego/amazonlinux-node10:1](https://hub.docker.com/repository/docker/syl20lego/amazonlinux-node/general])

  Build:

  ```
  docker build --rm --no-cache -t image-amazonlinux-build-docker-node10 ./amazonlinux-build-docker-node10/
  docker run -it image-amazonlinux-build-docker-node10 /bin/bash --name image-amazonlinux-build-docker-node10
  ```

  Publish:

  ```
  docker tag image-amazonlinux-build-docker-node10 syl20lego/amazonlinux-build-docker-node10:3
  docker push syl20lego/amazonlinux-build-docker-node10:3 --name amazonlinux-build-docker-node10
  ```

+ amazonlinux-node 12:
  AWS amzonelinux image node JS 12 for Fargate
  [syl20lego/amazonlinux-node12:1](https://hub.docker.com/repository/docker/syl20lego/amazonlinux-node/general])

  Build:

  ```
  docker build --rm --no-cache -t image-amazonlinux-build-docker-node12 ./amazonlinux-build-docker-node12/
  docker run -it image-amazonlinux-build-docker-node12 /bin/bash --name image-amazonlinux-build-docker-node12
  ```
  Publish:

  ```
  docker tag image-amazonlinux-build-docker-node12 syl20lego/amazonlinux-build-docker-node12:3
  docker push syl20lego/amazonlinux-build-docker-node12:3
  ```

 + amazonlinux-serverless-python36:
  AWS amzonelinux image node JS 12 for Fargate
  [syl20lego/amazonlinux-node12:1](https://hub.docker.com/repository/docker/syl20lego/amazonlinux-serverless/general])

 
  Build:

  ```
  docker build --rm --no-cache  -t image-amazonlinux-serverless-python36 ./amazonlinux-serverless-python36/
  docker run -it image-amazonlinux-serverless-python36 /bin/bash --name image-amazonlinux-serverless-python36 
  ```
  Publish:

  ```
  docker tag image-amazonlinux-serverless-python36 syl20lego/image-amazonlinux-serverless-python36:2
  docker push syl20lego/image-amazonlinux-serverless-python36:2
  ```


+ amazonlinux-build-awscli-node:
  AWS amzonelinux image with AWS CLI tools node JS 10 with yarn to build AWS lambda
  [syl20lego/amazonlinux-build-lambda10:1](https://hub.docker.com/repository/docker/syl20lego/amazonlinux-build-lambda/general])

+ amazonlinux-build-docker-node:
  AWS amzonelinux image with AWS CLI tools node JS 10 with yarn and docker, e.g. to build Fargate images
  [syl20lego/amazon-linux-build-docker10:2](https://hub.docker.com/repository/docker/syl20lego/amazonlinux-build-docker/general])
  Build:

  ```
  docker build --rm --no-cache  -t image-amazonlinux-build-awscli-node ./amazonlinux-build-awscli-node/
  docker run -it image-amazonlinux-build-awscli-node /bin/bash --name image-amazonlinux-build-awscli-node
  ```
  Publish:

  ```
  docker tag image-amazonlinux-build-awscli-node syl20lego/amazonlinux-build-awscli-node10:1
  docker push syl20lego/amazonlinux-build-awscli-node10:1
  ```


+ amazonlinux-node 10:
  AWS amzonelinux image node JS 10 for Fargate

  Build:

  ```
  docker build --rm --no-cache  -t image-amazonlinux-node ./amazonlinux-node/
  docker run -it image-amazonlinux-node /bin/bash --name image-amazonlinux-node
  ```
  Publish:

  ```
  docker tag image-amazonlinux-node syl20lego/amazonlinux-node10:1
  docker push syl20lego/amazonlinux-node10:1
  ```

