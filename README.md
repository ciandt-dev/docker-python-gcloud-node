# Python with Node env to run tests

Base image with:
- python 3.7.6
- node 12.14.1
- npm 6.13.6
- chromedriver 80.0.3987.16
- sonarscanner 4.2.0.1873
- java 8
- maven 3.6.3
- angular cli 8.2.14
- google-chrome

# Docker hub

[ciandt/docker-python-gcloud-node](https://hub.docker.com/r/ciandt/docker-python-gcloud-node/)

# Commands


## Build the image
```
docker build -t ciandt/docker-python-gcloud-node:[vN] .
```

## Push the image

```
docker push ciandt/docker-python-gcloud-node:[vN]
```

## Test local

```
docker run -it --volume=/Users/mendesdesouza/google-requisition-form:/localDebugRepo --workdir="/localDebugRepo" --memory=4g --memory-swap=4g --memory-swappiness=0 --entrypoint=/bin/bash ciandt/docker-python-gcloud-node
```

vN -> Is the docker version
