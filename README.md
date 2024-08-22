# Combostrap.com Website

## About

This repository contains the [https://combostrap.com](https://combostrap.com) 
written as [combo site](https://combostrap.com/admin/combostrap-website-yfi22ewn) 

## How to Run

To get the `Combostrap` website available at http://localhost:8081, execute:
```bash
docker run \
  --name site-com-combostrap \
  --rm \
  -p 8081:80 \
  -e DOKU_DOCKER_GIT_SITE=https://github.com/ComboStrap/site-com-combostrap \
  ghcr.io/combostrap/dokuwiki:php8.3-latest
```

## How to develop it

See [dev](docs/dev.md)