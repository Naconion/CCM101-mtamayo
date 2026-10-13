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
