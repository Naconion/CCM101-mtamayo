# Mission Overview

Congratulations! Your flawless work in deploying data storage solutions has earned you a spot on the
Cloud Deployment Team at CloudNova Technologies. Up until now, you have been deploying single containers (like a standalone web server or a storage
bucket). However, real-world enterprise applications are rarely just one container. They are "multi-tier" systems that require a frontend web application communicating seamlessly with a backend database. Deploying these one by one manually is prone to error. Enter Docker Compose. In this mission, you will transition from manual commands to Infrastructure as Code (IaC). Using a YAML configuration file, you will define a multi container private cloud storage application (Nextcloud and MariaDB) and deploy the entire stack simultaneously with a single command! Remember: A junior engineer deploys servers by typing commands; a senior engineer deploys infrastructure by writing code.

## Mission Objectives
At the end of this laboratory activity, you should be able to:
- Explain the concept of a multi-tier application architecture.
- Understand the purpose and structure of a docker-compose.yml file.
- Use a Linux command-line text editor (nano) to create configuration files.
- Deploy a multi-container application (Nextcloud + Database) using Docker Compose.
- Document deployment procedures and Infrastructure as Code (IaC) principles using Markdown.
- Continue expanding your professional GitHub Cloud Computing Portfolio.
## Required Resources / Tools used
- KillerCoda Playground (Ubuntu or Docker environment)
- GitHub Account
- Modern Web Browser
- Stable Internet Connection
## Commands Executed
* `mkdir nextcloud-deployment` - Creates a new project directory for the deployment configuration[cite: 2, 3].
* `cd nextcloud-deployment` - Navigates into the newly created project directory[cite: 2, 3].
* `nano docker-compose.yml` - Opens the Linux nano text editor to create and edit the Docker Compose configuration file[cite: 3].
* `docker-compose up -d` - Pulls the required container images, creates the network, and deploys the multi-tier application stack in the background[cite: 3, 4].
* `docker-compose ps` - Verifies that both the database and application containers are running successfully[cite: 3].
* `docker-compose down` - Gracefully stops and removes the entire container infrastructure stack[cite: 4].

## Skills Learned
* **Multi-Tier Architecture Design:** Understanding the separation of concerns between a front-end application tier and a backend database tier[cite: 1, 2].
* **Infrastructure as Code (IaC):** Defining multi-container environments declaratively using structured YAML configuration files rather than manual CLI commands[cite: 1, 3, 4].
* **Container Orchestration & Networking:** Utilizing Docker Compose to automatically link independent containers, manage environment variables, and configure internal hostname resolution[cite: 3, 4].
* **Linux Terminal Editing:** Practicing file creation and editing directly within a Linux server environment using the `nano` text editor[cite: 1, 3].
* **Technical Documentation:** Documenting deployment workflows, YAML code structures, and architecture principles using Markdown for a professional cloud portfolio[cite: 1, 2, 4].
