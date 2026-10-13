# MinIO Server Deployment Documentation #

## Deployment Overview ##
This document outlines the technical steps and configuration used to deploy an S3-compatible object storage server (MinIO) inside the Docker environment.

## Docker Deployment Command ##
The server was deployed using the following command:

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
  -e "MINIO_ROOT_USER=cloudadmin" \
  -e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
  chainguard/minio:latest server /data --console-address ":9001"
```
## Other technical steps done to achieve this ##
- In your KillerCoda Playground, locate the "Traffic / Ports" or "Custom Ports" tab (usually found on the
side or top menu of the interface).
- Enter port 9001 and click "Access" to open the MinIO Web Console in a new browser tab.
- Log in using the credentials you defined in the Docker command
- Once logged in, navigate to Buckets on the left menu and click Create Bucket.
- Name your bucket client-photos and save it.


## A brief explanation of what the -e flags (Environment Variables) did in your Docker command ##
In the Docker command, the -e flags are used to pass environment variables directly into the container upon startup, which allows you to configure essential settings dynamically without modifying the container's source code. Specifically, the -e "MINIO_ROOT_USER=cloudadmin" flag defines the administrator username (cloudadmin), while the -e "MINIO_ROOT_PASSWORD=CloudNova2026!" flag sets the secure password for that administrator account. Together, these environment variables establish the mandatory login credentials required to authenticate and securely access the MinIO Web Console and storage server.
