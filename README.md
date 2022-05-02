# DockerComposeFile

### cat usage

```shell
cat > docker-compose.yml <<EOF
version: "3.7"
services:
  nginx:
    image: nginx:alpine
    container_name: nginx
    restart: unless-stopped
    volumes:
      - ./html:/usr/share/nginx/html:ro
    ports:
      - 180:80
EOF
```

### docker-compose up -f

```shell
docker-compose -f docker-compose.yml up -d
```
