# Project Setup
This project had been tested on Ubuntu 22.04.3 LTS

1. Install Docker Engine: https://docs.docker.com/engine/install/ (select your OS)

2. Install Docker-Compose (e.g. Ubuntu: https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-compose-on-ubuntu-20-04)

3. Start docker service if it is necessary.

4. Create network for docker-compose services: "docker network create app-network"

5. Set DOCKERFILE environment variable(you can choose between Dockerfile.dev and Dockefile.prod. Depends on this application will run in development mode or production mode): "export DOCKERFILE=Dockerfile.dev"

6. "docker-compose build --pull --no-cache"

7. "docker-compose up -d"

8. Backend will be visible on the port 80.

MariaDB database will be available only from the php container.

```sh
composer install
```
  