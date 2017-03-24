# dockerized-docs-keepalived

# What is it?
Dockerzied Keepalived documentation for offline use.

# Image description #
- Base image: `fedora:latest`.
- The keepalived `master` branch is cloned and docs are built using sphinx.
- Httpd server is installed
- Keepalived documentation directory (`/keepalived/doc/build/html`) is linked to httpd `DocumentRoot` (`/var/www/html`).

# How to use this image #

```console
$ docker run -d genadipost/keepalived

```
You can test it by visiting http://container-ip:80
