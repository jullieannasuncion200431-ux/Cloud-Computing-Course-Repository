# Mission 6: Cloud Deployment Engineer

## Mission Overview
This mission focuses on deploying a multi-tier cloud application using Docker Compose. The project uses Nextcloud as the web application and MariaDB as its database.

## Objectives
- Understand two-tier architecture.
- Create a Docker Compose YAML configuration.
- Deploy and manage multiple containers.
- Access the Nextcloud web interface through port 8080.
- Document Infrastructure as Code (IaC) and Docker Compose concepts.

## Commands Executed
```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose down
```

## Skills Learned
- Understanding web/application and database tiers.
- Writing YAML configuration files.
- Deploying multi-container applications.
- Managing containers using Docker Compose.
- Accessing a containerized web application.
- Writing technical documentation in Markdown.
- Organizing and maintaining a GitHub cloud computing portfolio.

## Project Files
- `multi-tier-architecture.md` — Explains the two-tier architecture.
- `docker-compose-guide.md` — Documents the Docker Compose configuration.
- `reflection.md` — Describes lessons learned during the mission.
- `screenshots/` — Contains deployment, browser, and teardown evidence.
