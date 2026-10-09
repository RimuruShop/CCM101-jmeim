## Laboratory Activity 7: Mission 7 – The Cloud Operations Engineer

Mission Overview
This lab focuses on observability — establishing a host server’s baseline health, deploying a containerized Nginx web server, generating both normal and error traffic against it, and using Docker’s logging and metrics tools to prove the infrastructure is healthy and ready for a traffic surge.

##Objectives

Use native Linux CLI tools to monitor host CPU, memory, and disk capacity
Deploy a web container and track its real-time performance
Generate web traffic and extract application access logs for analysis
Translate raw performance data into a readable technical report

##Monitoring Commands Executed

free -h — check memory usage
df -h — check disk storage
top — view live CPU load and running processes
docker run -d --name client-website -p 8080:80 nginx — deploy the container
curl http://localhost:8080 — simulate normal traffic
curl http://localhost:8080/hidden-admin-page — simulate a broken request
docker logs client-website — retrieve application logs
docker stats — view real-time container resource usage

##Skills Learned

Establishing a host-level performance baseline before deployment
Generating and reading HTTP access logs, including error codes
Reading live container resource metrics (CPU, memory, network I/O)
Understanding the difference between monitoring (metrics) and logging (events)
