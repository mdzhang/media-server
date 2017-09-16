# media-server

Dockerized stuff for a home media server.

## Configuring Environment variables

##### PGID and PUID

See [here](https://hub.docker.com/r/linuxserver/sickrage/) for more on User/Group identifiers.

TL;DR

```
$ whoami
mdzhang
$ id mdzhang
uid=501(mdzhang) gid=20(staff) groups=...
```

`PUID` == 501
`PGID` == 20

## File Organization

Assumes

```
- $HOME
    \_ media
        \_ data
            \_ tv
            \_ movies
        \_ config
            \_ plex
        \_ tmp
```

## Usage

1. Review config values
1. Confirm file organization
1. Confirm you have installed and started Docker for Mac
1. Bring up services

```
$ cp .env.sample .env
$ make up
```
