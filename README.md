[![Docker build images](https://github.com/dmmeteo/docker-htpasswd/actions/workflows/docker.yml/badge.svg)](https://github.com/dmmeteo/docker-htpasswd/actions/workflows/docker.yml)

# htpasswd

## Usage

To generate a password file:

```shell
docker run --rm -ti dmmeteo/htpasswd <username> <password> > htpasswd
```

This will use bcrypt encryption.

## Build

To rebuild for all platforms:

```shell
docker buildx build \
    --platform=linux/amd64,linux/arm64,linux/ppc64le,linux/s390x,linux/386,linux/arm/v7,linux/arm/v6 \
    -t dmmeteo/htpasswd:latest . --push
```
