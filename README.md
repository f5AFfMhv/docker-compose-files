# Docker compose files for various services

## Running services

1. Install [docker](https://docs.docker.com/engine/install/) and [compose](https://docs.docker.com/compose/install/linux/) plugin or standalone [docker-compose](https://pypi.org/project/docker-compose/).
2. Some compose files have variables that should be defined in `.env` file. Look into `.env_example`.
3. Run

```bash
sudo docker compose -f <SERVICE>.yaml --env-file .env up -d
```

## Using Caddy as reverse proxy

Services are configured to run behind caddy reverse proxy. If you want to run them standalone, uncomment `port` section in yaml file and remove external network section:

```yaml
networks:
  default:
    external:
      name: caddy-network
```

To run services behind Caddy:

1. Create self-signed certificate in `${config_dir}/caddy` directory

```bash
openssl genpkey -algorithm RSA -out server.key
openssl req -new -x509 -key server.key -out server.crt -days 365
```

2. Add `Caddyfile` configuration file to the same directory

```
# example Caddyfile

*.home.lab {
    tls /server.crt /server.key
}

files.home.lab {
  reverse_proxy filebrowser:8080
}
kavita.home.lab {
  reverse_proxy kavita:5000
}
```

3. Add records to DNS server or yout `hosts` file

```bash
# /etc/hosts
192.168.0.10 files.home.lab kavita.home.lab
```

4. Create docker network

```bash
sudo docker network create caddy-network
```

5. Start caddy from `caddy.yaml`.

Now filebrowser container can be reached on https://files.home.lab.
