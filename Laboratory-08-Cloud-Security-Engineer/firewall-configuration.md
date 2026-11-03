# Firewall Configuration

## Allow Port 8080 (Web Application)

```
sudo ufw allow 8080/tcp
```

This command allows incoming TCP traffic through port 8080, making the web application accessible to users.

## Check Firewall Status

```
sudo ufw status numbered
```

The command displays the active firewall rules. Based on the screenshot, SSH (22/tcp) and port 8080 are allowed for both IPv4 and IPv6.

## Test Nginx Web Server

```
curl http://localhost:8080/
```

This command checks if the Nginx web server is running correctly. The output displays the default Nginx welcome page, confirming that the server is working properly.

