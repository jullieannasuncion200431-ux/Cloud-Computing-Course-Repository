# Docker Compose Guide

## 1. The `services:` Block
The `services:` block defines the containers or services that make up an application. In this project, it defines two services: `database`, which uses the MariaDB 10.6 image, and `app`, which uses the Nextcloud image.

# The Compose File Used

version: '3'
services:
  database:
    image: mariadb:10.6
    environment:
      - MYSQL_ROOT_PASSWORD=cloudnova_root
      - MYSQL_PASSWORD=cloudnova_pass
      - MYSQL_DATABASE=nextcloud_db
      - MYSQL_USER=nextcloud_user
      
  app:
    image: nextcloud
    ports:
      - 8080:80
    environment:
      - MYSQL_PASSWORD=cloudnova_pass
      - MYSQL_DATABASE=nextcloud_db
      - MYSQL_USER=nextcloud_user
      - MYSQL_HOST=database

## 2. Environment Variables
Environment variables configure the containers when they start.

- `MYSQL_ROOT_PASSWORD` sets the MariaDB root password.
- `MYSQL_PASSWORD` specifies the password for the Nextcloud database user.
- `MYSQL_DATABASE` specifies the database name.
- `MYSQL_USER` specifies the database username.
- `MYSQL_HOST=database` tells Nextcloud to connect to the database service named `database`.

Docker Compose provides service-name-based networking so that the application can reach the database using its service name.

**Security note:** The example uses passwords directly in the YAML file for learning purposes. In a real deployment, use secure secrets management and avoid committing actual passwords to a public repository.

## 3. Docker Compose Configuration
The `database` service uses `mariadb:10.6`. The `app` service uses the `nextcloud` image and maps host port 8080 to container port 80 using `8080:80`. This allows the web interface to be accessed through port 8080.

## 4. Docker Run vs. Docker Compose

### Docker Run
The `docker run` command starts and configures an individual container. When several containers are required, separate commands may be needed to configure their ports, environment variables, networks, and relationships.

### Docker Compose
The `docker-compose up -d` command reads the Compose YAML file and starts the services defined in it. The `-d` option runs the containers in the background. Compose makes multi-container deployments easier to repeat and manage.

## 5. Useful Commands

```bash
docker-compose up -d
docker-compose ps
docker-compose logs
docker-compose down
```

- `up -d` starts the application stack in the background.
- `ps` displays the Compose containers and their status.
- `logs` displays service logs to help with troubleshooting.
- `down` stops and removes the containers and the Compose network.

## Conclusion
Docker Compose is an Infrastructure as Code tool that allows engineers to define and manage a multi-container application using a readable configuration file.
