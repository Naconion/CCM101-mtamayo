# Laboratory Activity 02: Build the Cloud Infrastructure Blueprint

## Mission Overview
In this lab, I took on the role of a cloud engineer preparing an infrastructure assessment for a client migrating to the cloud. Working inside a temporary Linux server provided by KillerCoda, I explored system resources, identified core cloud building blocks, mapped services across major cloud vendors, created a foundational architecture diagram, and documented my findings on GitHub[cite: 1].

## Objectives
* Explore hardware and software resources inside a virtualized Linux environment[cite: 1].
* Explain how compute, storage, networking, and identity components function in cloud architecture[cite: 1].
* Compare equivalent core services offered by AWS, Azure, and Google Cloud[cite: 1].
* Draw a basic, end-to-end cloud infrastructure diagram[cite: 1].
* Maintain clean technical documentation using Markdown and Git[cite: 1].

## Cloud Infrastructure Components
During my server inspection, I mapped the Linux environment to four primary cloud building blocks[cite: 1]:
* **Compute:** Handled by virtualized CPU cores and allocated RAM to process system workloads[cite: 1].
* **Storage:** Provided by block storage and file systems mounted at root (`/`) to keep files persistent[cite: 1].
* **Networking:** Managed through virtual network interfaces, hostnames, and IP addressing for server communications[cite: 1].
* **Operating System:** Supported by the Ubuntu Linux distribution and kernel, providing the runtime environment for software[cite: 1].

## Tools Used
* **KillerCoda Terminal:** Hosted cloud Linux sandbox[cite: 1].
* **GitHub:** Version control and portfolio hosting[cite: 1].
* **Excalidraw / Draw.io:** Cloud architecture diagram design[cite: 1].
* **VS Code / Markdown:** Writing technical documentation[cite: 1].

## Linux Commands Executed
Here are the primary commands I used to gather hardware and network details from the server[cite: 1]:

| Command | Purpose |
| :--- | :--- |
| `cat /etc/os-release` | Checked the installed Linux operating system distribution[cite: 1]. |
| `uname -r` | Retrieved the Linux kernel version[cite: 1]. |
| `lscpu` | Displayed CPU architecture, model name, and core counts[cite: 1]. |
| `free -h` | Monitored total, used, and available system memory (RAM)[cite: 1]. |
| `df -h` | Inspected mounted disk partitions and available storage space[cite: 1]. |
| `hostname` | Identified the server's network name[cite: 1]. |
| `ip a` | Listed virtual network interfaces and assigned IP addresses[cite: 1]. |

## Skills Learned
* Using standard Linux CLI utilities to inspect virtualized infrastructure[cite: 1].
* Mapping physical/virtual server specs to abstract cloud infrastructure concepts[cite: 1].
* Translating infrastructure components across AWS, Azure, and GCP terminology[cite: 1].
* Structuring clean, professional engineering reports using Markdown[cite: 1].

## Challenges Encountered
* **Reading CLI Output:** Sorting through dense output from commands like `lscpu` and `ip a` to find specific metrics required careful reading.
* **Diagram Layout:** Organizing the flow from user to network and storage clearly without making the architecture look cluttered took a couple of attempts.
