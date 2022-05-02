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
