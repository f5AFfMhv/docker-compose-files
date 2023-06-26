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
  <a href=https://hub.docker.com/r/pawelmalak/flame>Flame</a> is self-hosted startpage for your server.
</details>
<details>
  <summary>Gitea - RPI</summary>
  <a href=https://about.gitea.com/>Gitea</a> is a lightweight DevOps platform.
</details>
<details>
  <summary>Librespeed - RPI</summary>
  <a href=https://librespeed.org/>Librespeed</a> is free and Open Source Speedtest.
</details>
<details>
  <summary>Nextcloud - RPI</summary>
  <a href=https://nextcloud.com/>Nextcloud</a> is self-hosted collaboration solution.
</details>
<details>
  <summary>NordVPN proxy - RPI</summary>
  Alpine image with OpenVPN and Privoxy to use with your NordVPN account.
</details>
<details>
  <summary>NPM - RPI</summary>
  Docker container for managing <a href=https://nginxproxymanager.com/>NPM</a> hosts with a simple, powerful interface.
</details>
<details>
  <summary>Pihole - RPI</summary>
  <a href=https://pi-hole.net/>Pihole</a> is a DNS sinkhole that protects your devices from unwanted content, without installing any client-side software.
</details>
<details>
  <summary>Plex - RPI</summary>
  <a href=https://www.plex.tv/>Plex</a> combines free movies & TV with your favorite streaming services.
</details>
<details>
  <summary>Portainer - RPI</summary>
  <a href=https://www.portainer.io/>Portainer</a> is powerful container management.
</details>
<details>
  <summary>RPI monitor - RPI</summary>
  Grafana dashboard for raspberry pi.
  Based on <a href=https://github.com/novaspirit/Docker-Raspberry-PI-Monitoring>this</a> project and expanded with <a href=https://github.com/f5AFfMhv/emonesp-grafana>this</a>.
</details>
<details>
  <summary>Seafile - RPI</summary>
  <a href=https://www.seafile.com/en/home/>Seafile</a> is an open source file sync&share solution.
</details>
<details>
  <summary>Syncthing - RPI</summary>
  <a href=https://syncthing.net/>Syncthing</a> is a continuous file synchronization program.
</details>
<details>
  <summary>Traefik - RPI</summary>
  <a href=https://traefik.io/>Traefik</a> is cloud-native application proxy.
</details>
<details>
  <summary>Vikunja - RPI</summary>
  <a href=https://vikunja.io/>Vikunja</a> is the open-source, self-hostable to-do app.
</details>