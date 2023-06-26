# Docker compose files for various services
Compose files in `rpi_compose_files` directory are tested on Raspberry Pi 4.
1. Install docker and docker-compose plugin (or standalone docker-compose version).
2. Some compose files have variables that should be defined in `.env` file.
3. Run
```bash
docker compose -f <FILE NAME> up -d
```

# Service list
<details>
  <summary>Flame - RPI</summary>
  [Flame](https://hub.docker.com/r/pawelmalak/flame) is self-hosted startpage for your server.
</details>
<details>
  <summary>Gitea - RPI</summary>
  [Gitea](https://about.gitea.com/) is a lightweight DevOps platform.
</details>
<details>
  <summary>Librespeed - RPI</summary>
  [Librespeed](https://librespeed.org/) is free and Open Source Speedtest.
</details>
<details>
  <summary>Nextcloud - RPI</summary>
  [Nextcloud](https://nextcloud.com/) is self-hosted collaboration solution.
</details>
<details>
  <summary>NordVPN proxy - RPI</summary>
  Alpine image with OpenVPN and Privoxy to use with your NordVPN account.
</details>
<details>
  <summary>NPM - RPI</summary>
  Docker container for managing [Nginx proxy](https://nginxproxymanager.com/) hosts with a simple, powerful interface.
</details>
<details>
  <summary>Pihole - RPI</summary>
  [Pi-hole®](https://pi-hole.net/) is a DNS sinkhole that protects your devices from unwanted content, without installing any client-side software.
</details>
<details>
  <summary>Plex - RPI</summary>
  [Plex](https://www.plex.tv/) combines free movies & TV with your favorite streaming services.
</details>
<details>
  <summary>Portainer - RPI</summary>
  [Portainer](https://www.portainer.io/) is powerful container management.
</details>
<details>
  <summary>RPI monitor - RPI</summary>
  Grafana dashboard for raspberry pi.
  Based on [this](https://github.com/novaspirit/Docker-Raspberry-PI-Monitoring) project.
  Expanded with [this](https://github.com/f5AFfMhv/emonesp-grafana).
</details>
<details>
  <summary>Seafile - RPI</summary>
  [Seafile](https://www.seafile.com/en/home/) is an open source file sync&share solution.
</details>
<details>
  <summary>Syncthing - RPI</summary>
  [Syncthing](https://syncthing.net/) is a continuous file synchronization program.
</details>
<details>
  <summary>Traefik - RPI</summary>
  [Traefik](https://traefik.io/) is cloud-native application proxy.
</details>
<details>
  <summary>Vikunja - RPI</summary>
  [Vikunja](https://vikunja.io/) is the open-source, self-hostable to-do app.
</details>