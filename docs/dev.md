# How to develop the ComboStrap Website


## On Windows WSL, Linux or macOS

On your desktop:
```bash
git clone https://github.com/ComboStrap/site-com-combostrap
cd site-com-combostrap
docker run \
  --name site-com-combostrap \
  --rm \
  -p 8081:80 \
  --user 1000:1000 \
  -e DOKU_DOCKER_ENV=dev \
  -e DOKU_DOCKER_ACL_POLICY='public' \
  -e DOKU_DOCKER_ADMIN_NAME='admin' \
  -e DOKU_DOCKER_ADMIN_PASSWORD='welcome' \
  -v $PWD:/var/www/html \
  ghcr.io/combostrap/dokuwiki:php8.3-latest
```
The ComboStrap site should be available at: http://localhost:8081


## Wanted Page Check


```bash
docker exec -it site-com-combostrap php ./bin/wantedpages.php
```