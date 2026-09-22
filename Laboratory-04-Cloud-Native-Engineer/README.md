# LABORATORY-04-CLOUD-NATIVE-ENGINEER

## Mission Overview

Congratulations! After successfully guiding our clients through multi-cloud evaluations, you have been
promoted to the Cloud-Native Engineering Team at CloudNova Technologies.
Modern cloud computing is no longer just about renting Virtual Machines (VMs) from AWS or Azure. Today's
enterprise applications are built using lightweight, portable, and lightning-fast technologies called Containers.
Your new mission is to understand the shift from traditional virtualization to containerization.
Using the KillerCoda Playground, you will step into the shoes of a Cloud-Native Engineer. You will research the
differences between VMs and containers, execute your very first Docker commands, and deploy a live,
containerized web server in seconds.
Remember: A traditional system administrator manages servers, but a cloud-native engineer manages
the services running on them.

## Mission Objectives
At the end of this laboratory activity, you should be able to:
- Differentiate between traditional Virtual Machines (VMs) and Containers.
- Access a Docker-enabled cloud environment using KillerCoda.
- Execute fundamental Docker CLI (Command Line Interface) commands.
- Pull, run, manage, and terminate a containerized application (Nginx).
- Create professional technical documentation of container operations using Markdown.
- Continue developing a well-organized GitHub Cloud Computing Portfolio.

## Required Resources
- KillerCoda Playground (Ubuntu or Docker environment)
- GitHub Account
- Modern Web Browser
- Stable Internet Connection

## **Docker Commands Executed** (List all the commands you used in Checkpoints 3, 4, and 5)

*Checkpoint 3*

**docker --version**

**docker info**

*Checkpoint 4*

**docker pull nginx**

**docker run -d -p 8080:80 --name nginx-server nginx**

**curl http://localhost:8080**

*Checkpoint 5*

**docker ps**

**docker stop nginx-server**

**docker ps -a**

**docker rm nginx-server**


## Skills Learned

I learned how to use basic Docker commands in a Linux environment. I learned how to download and run an Nginx container, map a host port to a container port, and test a web server using curl. I also learned how to check, stop, and remove Docker containers using Docker CLI commands. This activity helped me understand how containers can be used to deploy applications quickly and efficiently.

## Challenges Encountered

One challenge I encountered was entering the Docker commands correctly. While testing the Nginx web server, I accidentally entered an extra ~ after port 8080 in the curl command, which caused an error. I corrected the command by using curl http://localhost:8080, which allowed me to successfully test the Nginx web server. I also needed to understand how port mapping connects port 8080 on the host to port 80 inside the container.
