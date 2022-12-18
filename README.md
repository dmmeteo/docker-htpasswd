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
docker buildx build --platform=linux/amd64,linux/arm64,linux/arm/v7 -t dmmeteo/htpasswd:latest . --push
```
