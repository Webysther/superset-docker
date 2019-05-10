[![Software License](https://goo.gl/FU2Kw1)](LICENSE)

# Docker for [Superset](https://github.com/apache/incubator-superset)

Projeto que permite enviar o superset para produção com apenas um docker e com os banco de dados mais comuns. Uma mistura de [amancevice/superset](https://hub.docker.com/r/amancevice/superset) com [tylerfowler/superset](https://hub.docker.com/r/tylerfowler/superset) ([github](https://github.com/tylerFowler/docker-superset)).

## Usage

Build:

```bash
docker build .
```

Use:

```bash
docker run -d --name superset \
  -e ADMIN_USERNAME=myadminuser \
  -e ADMIN_FIRST_NAME=Some \
  -e ADMIN_LAST_NAME=Name \
  -e ADMIN_EMAIL=nobody@nowhere.com \
  -e ADMIN_PWD=mypassword \
  -p 8088:8088 \
webysther/superset
```
