# MinIO Deployment Documentation

## Docker Command Used

`docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \ -e "MINIO_ROOT_USER=cloudadmin" \ -e "MINIO_ROOT_PASSWORD=CloudNova2026!" \ minio/minio server /data --console-address ":9001"`

## Port Used to Access the Web Console

Port **9001** was used to access the MinIO Web Console. It was opened through KillerCoda's **"Traffic/Ports"** tab, which allowed the console to be accessed through a web browser.

## Bucket Created

**client-photos**

## What the `-e` Flags Did

The `-e` flag is used to set environment variables when the MinIO container starts. In this command:

- `MINIO_ROOT_USER=cloudadmin` sets the username used to access the MinIO admin console.
- `MINIO_ROOT_PASSWORD=CloudNova2026!` sets the password used to log in to the MinIO console.

These environment variables allow the login credentials to be configured when the container is created. This makes the MinIO setup easier to reuse and modify for different deployments.
