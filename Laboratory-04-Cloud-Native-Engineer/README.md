# Laboratory 04: Cloud-Native Engineer

## Mission Overview
This lab covers the transition from traditional Virtual Machines to containerized applications using Docker. It includes researching VM vs. container architecture, deploying a live Nginx container, and managing its lifecycle.

## Objectives
- Differentiate between VMs and Containers
- Access a Docker-enabled environment using KillerCoda
- Execute fundamental Docker CLI commands
- Pull, run, manage, and terminate a containerized application (Nginx)
- Document container operations in Markdown

## Docker Commands Executed
```bash
docker --version
docker info
docker pull nginx
docker run -d -p 8080:80 --name my-nginx nginx
curl http://localhost:8080
docker ps
docker stop my-nginx
docker ps -a
docker rm my-nginx
```

## Skills Learned
- Verifying a Docker environment's installation and status
- Pulling images from Docker Hub
- Running containers in detached mode with port mapping
- Managing the full container lifecycle (list, stop, verify, remove)

## Challenges Encountered

While testing the Nginx container, I encountered an issue when I clicked the `curl http://localhost:8080` command in the KillerCoda instructions. Instead of running in the KillerCoda terminal, it opened in my local browser and showed an **ERR_CONNECTION_REFUSED** error. I realized that `localhost` refers to the machine where the command is being executed. Since the Nginx container was running on KillerCoda's remote virtual machine, my local computer could not access it through `localhost:8080`. I solved the problem by manually typing the `curl http://localhost:8080` command into the KillerCoda terminal, which successfully displayed the **"Welcome to nginx!"** output. This helped me understand how `localhost` works and the difference between my local computer and a remote virtual machine.

