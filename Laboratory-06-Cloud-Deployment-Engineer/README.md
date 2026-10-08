# Laboratory Activity 6: Mission 6 – The Cloud Deployment Engineer

## Mission Overview

This laboratory activity focuses on Infrastructure as Code (IaC) using Docker Compose. It involves setting up a two-tier private cloud storage system using Nextcloud and MariaDB through one YAML configuration file instead of manually creating each container.

## Objectives

- Describe the structure of a multi-tier application
- Understand the role and organization of a `docker-compose.yml` file
- Use Nano to create and edit configuration files through the terminal
- Deploy several containers using Docker Compose
- Record deployment steps and explain IaC concepts using Markdown

## Commands Executed

- `mkdir nextcloud-deployment` – created the deployment folder
- `cd nextcloud-deployment` – entered the project directory
- `nano docker-compose.yml` – created and edited the Compose configuration
- `docker-compose up -d` – started the containers
- `docker-compose ps` – checked the running containers
- `docker-compose down` – stopped and removed the containers

## Skills Learned

- Creating properly formatted and indented YAML files
- Running multiple connected containers using a single Docker Compose command
- Understanding how Docker Compose networking allows containers to communicate through service names
- Creating clear Infrastructure as Code documentation for other developers

Available next action: Create a downloadable DOCX file here in this chat containing the editable prose above
