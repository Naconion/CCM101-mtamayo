# Mission Overview
This onboarding laboratory activity provides hands-on experience setting up a cloud-based Linux server environment using KillerCoda's Ubuntu 24.04 platform. It focuses on foundational system administration tasks, Linux command-line navigation, system diagnostic reporting, and setting up a professional GitHub repository for tracking coursework deliverables.

# Objectives
- Provision and configure a cloud-hosted Ubuntu 24.04 Linux instance.
- Create a dedicated user account with administrator privileges.
- Execute diagnostic commands to gather hardware, OS, and resource metrics.
- Build a structured workspace directory layout for storing cloud deliverables.
- Maintain continuous technical documentation using Markdown and Git version control.

# Activities Performed
1. **Environment Setup:** Launched an Ubuntu 24.04 playground on KillerCoda, created the user account `mtamayo`, assigned `sudo` privileges, and logged into the user session.
2. **System Profiling:** Ran diagnostic tools to gather details on system architecture, memory usage, disk allocation, kernel version, and OS details into `system-information.md`.
3. **Workspace Building:** Created standard workspace directories (`Documents`, `Notes`, `Reports`, `Screenshots`) and drafted a personal biography file (`about-me.md`).
4. **Portfolio Setup:** Established the public GitHub repository `CCM101-mtamayo` and added a root `README.md`.
5. **Documentation & Deliverables:** Structured the `Laboratory-01-Welcome-to-the-Cloud` directory, drafted `reflection.md`, organized captured evidence under `screenshots/`, and committed changes to GitHub.

# Linux Commands Used
* `useradd`, `passwd`, `usermod`: Created user `mtamayo` and granted administrative (`sudo`) access.
* `su`: Switched active shell user to `mtamayo`.
* `uname`, `cat /etc/os-release`, `lscpu`: Queried kernel version, distribution info, and CPU hardware details.
* `free -h`, `df -h`: Checked total RAM allocation and available disk space in human-readable formats.
* `mkdir`, `mv`, `cp`: Managed directory structure and organized activity files.
* `nano`, `cat`: Created, edited, and verified Markdown documentation files.
* `git add`, `git commit`, `git push`: Tracked and published laboratory assets to GitHub.

# Skills Learned
* **Cloud CLI Navigation:** Operating within web-based Linux virtual environments using standard terminal commands.
* **User & Security Administration:** Provisioning accounts and managing privilege elevation in Linux.
* **Resource Monitoring:** Gathering hardware and operating system metrics for infrastructure auditing.
* **Technical Documentation:** Authoring formatted Markdown logs and managing version-controlled portfolios on GitHub.
