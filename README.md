# Homelab Boilerplates

Starter configurations for common homelab services. Each config is production-ready with security defaults, designed to be dropped into a Docker Compose stack and customized for your environment.

## Configs

| File | Service | Description |
|------|---------|-------------|
| `YAML-configs/authentik.yml` | [Authentik](https://goauthentik.io/) | Identity provider and SSO — server, worker, PostgreSQL, Redis |
| `YAML-configs/docker-compose.yml` | Docker Compose | Multi-service stack template with networking and volume patterns |
| `YAML-configs/traefik.yaml` | [Traefik](https://traefik.io/) | Reverse proxy with Let's Encrypt, middleware chains, Docker provider |

## Usage

1. Copy the config you need into your project
2. Replace placeholder values with your environment-specific settings
3. Create required `.env` files for secrets (never commit secrets to git)
4. Deploy with `docker compose up -d`

## Part of ValkyrieNexus Homelab

These boilerplates are extracted from a production homelab running Proxmox VE, Docker, K3s, Traefik, Authentik, and Wazuh. See [valkyrienexus.dev](https://valkyrienexus.dev) for architecture docs and runbooks.

## License

MIT
