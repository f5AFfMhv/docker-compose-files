# Docker compose files for various services

1. Install [docker](https://docs.docker.com/engine/install/) and [compose](https://docs.docker.com/compose/install/linux/) plugin or standalone [docker-compose](https://pypi.org/project/docker-compose/).
2. Some compose files have variables that should be defined in `.env` file. Look into `.env_example`.
3. Run

```bash
sudo docker compose -f <SERVICE>.yaml --env-file .env up -d
```
