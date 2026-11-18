# homelab
Home server setup with Docker and monitoring 🖥️

## Stack
- **Server:** Ubuntu Server 26.04
- **Containers:** Docker, Docker Compose
- **Access:** SSH keys, Tailscale, ufw
- **Monitoring:** Node Exporter → Prometheus → Grafana → Telegram alerts

## Features

- 🚧 Monitoring: alerts for disk, RAM and battery

## Run
Check [monitoring/.env.example](monitoring/.env.example) and set it in your `monitoring/.env`
```bash
cd monitoring
cp .env.example .env
nano .env
docker compose up -d
```
Grafana: `http://<server-ip>:3000`