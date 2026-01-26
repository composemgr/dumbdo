## 👋 Welcome to dumbdo 🚀

Simple to-do list and task management

## 📋 Description

Simple to-do list and task management

## 🚀 Services

- **app**: dumbwareio/dumbdo:latest

## 📦 Installation

### Option 1: Quick Install
```bash
curl -q -LSsf "https://raw.githubusercontent.com/composemgr/dumbdo/main/docker-compose.yaml" -o compose.yml
```

### Option 2: Git Clone
```bash
git clone "https://github.com/composemgr/dumbdo" ~/.local/srv/docker/dumbdo
cd ~/.local/srv/docker/dumbdo
docker compose up -d
```

### Option 3: Using composemgr
```bash
composemgr install dumbdo
```

## 🔧 Configuration

### Environment Variables

```shell
TZ=America/New_York
APP_SECRET_PIN=changeme_pin_4_digits
APP_ORG_NAME=Dumbdo
```

See `docker-compose.yaml` for complete list of configurable options.

## 🌐 Access

- **Web Interface**: http://172.17.0.1:58062

## 📂 Volumes

- `./rootfs/data/dumbdo` - Data storage

## 🔐 Security

- Change all default passwords before deploying to production
- Use strong secrets for all authentication tokens
- Configure HTTPS using a reverse proxy (nginx, traefik, caddy)
- Regularly update Docker images for security patches
- Backup your data regularly

## 🔍 Logging

```shell
docker compose logs -f app
```

## 🛠️ Management

```bash
# Start services
docker compose up -d

# Stop services
docker compose down

# Update to latest images
docker compose pull && docker compose up -d

# View logs
docker compose logs -f

# Restart services
docker compose restart
```

## 📋 Requirements

- Docker Engine 20.10+
- Docker Compose V2+

## 🤝 Author

🤖 casjay: [Github](https://github.com/casjay) 🤖  
🦄 composemgr: [Github](https://github.com/composemgr) 🦄
