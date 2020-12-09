# Python with Node env to run tests

Base image with:
- python 3.8.6
- node 12.18.4
- npm 6.14.6
- chromedriver 80.0.3987.16
- sonarscanner 4.2.0.1873
- java 8
- maven 3.6.3
- angular cli 10.1.2
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
docker run -it --volume=/Users/mendesdesouza/google-requisition-form:/localDebugRepo --workdir="/localDebugRepo" --memory=2g --memory-swap=2g --memory-swappiness=0 --entrypoint=/bin/bash ciandt/docker-python-gcloud-node
```

vN -> Is the docker version
