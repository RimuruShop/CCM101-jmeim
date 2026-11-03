# Laboratory Activity 8: Mission 8 – The Cloud Security Engineer

## Mission Overview

This laboratory activity focuses on improving server security through defense-in-depth by using a host-based firewall. It involves setting up a web application, checking open network ports, and configuring UFW with a Default Deny policy. This ensures that only necessary connections are permitted while unauthorized traffic is blocked.

## Objectives

- Learn the importance of the Attack Surface and Principle of Least Privilege.
- Check and examine active network ports for possible security risks.
- Configure UFW using the Default Deny policy.
- Manage specific ports to allow SSH and web application traffic.

## Commands Executed

- `docker run -d --name secure-web-app -p 8080:80 nginx` — created and launched an Nginx web application accessible through port 8080.
- `sudo ufw allow ssh` — permitted SSH connections before turning on the firewall.
- `sudo ufw default deny incoming` / `sudo ufw default allow outgoing` — configured the firewall to block incoming traffic while permitting outgoing connections.
- `sudo ufw enable` — enabled the firewall protection.
- `sudo ufw status verbose` — checked the firewall status and its current configuration.
- `sudo ufw allow 8080/tcp` — permitted incoming connections through port 8080 for the web application.
- `sudo ufw status numbered` — displayed the firewall rules to verify that the new port permission was added.

## Skills Learned

- Setting up and managing a server firewall using the Default Deny policy.
- Understanding the importance of allowing SSH before activating the firewall.
- Controlling network access through specific ports to reduce security risks.
- Recording firewall configurations and security procedures for easier monitoring and future reference.
