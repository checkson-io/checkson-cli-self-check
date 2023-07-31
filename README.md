# Checkson self check for Checkson CLI

This check is used to monitor if the most recent version of [Checkson CLI](https://github.com/checkson-io/checkson-cli)
works and can communicate with the backend.

## Environment variables

| Variable                | Description |
|------------------------ |-------------|
| `VERSION`               | The version of the CLI to test |
| `PERSONAL_ACCESS_TOKEN` | The personal access token to login with |

## Use check on Checkson

This check can be used on [checkson.io](https://checkson.io) (or anywhere else) with the following Docker image:

```
ghcr.io/checkson-io/checkson-cli-self-check:main
```

## Run check locally

```
docker run \
  --env VERSION=1.0.0 \
  --env PERSONAL_ACCESS_TOKEN=abc123 \
  --rm \
  -it \
  ghcr.io/checkson-io/checkson-cli-self-heck:main
```
