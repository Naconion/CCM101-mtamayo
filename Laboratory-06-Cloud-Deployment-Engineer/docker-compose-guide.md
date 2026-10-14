# Docker Compose Technical Guide: Nextcloud & MariaDB Deployment

## Overview of the `services:` Block
The `services:` block acts as the core blueprint section in a `docker-compose.yml` file where you define all the individual containers that comprise your multi-tier application stack. Under this block, every indented entry (such as `database` and `app`) represents a distinct container service[cite: 3]. It specifies how each container should be built or pulled—including container images, environment configurations, and network port mappings—allowing Docker Compose to orchestrate and manage them as a unified system[cite: 3].

## Container Discovery: How Nextcloud Finds MariaDB
The Nextcloud application container locates and connects to the MariaDB database container via the environment variable:

```yaml
MYSQL_HOST=database
```
## What is the difference between docker run (which you used in Mission 4) and docker-compose up -d?
When Docker Compose deploys a stack, it automatically creates a dedicated internal network for the project and sets up built-in DNS resolution. Because the database service is explicitly named database in the configuration file, Docker's internal DNS maps the hostname database directly to the internal IP address of the MariaDB container. This allows the Nextcloud app container to seamlessly reach the database without needing hardcoded external IP addresses
