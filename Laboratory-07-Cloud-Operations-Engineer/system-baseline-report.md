# System Baseline Report

## 1. Host Resource Capacity
Below are the baseline hardware measurements captured from the Linux host server prior to application deployment.

* **Total Available RAM:** 1.9Gi
* **Total Storage Capacity (Root `/` File System):** 19G

## 2. Disk Space Criticality Analysis
* **Why checking disk space is critical before a massive traffic surge:** Checking disk space is critical before a massive traffic surge to ensure the server does not run out of storage when writing growing application logs, cache files, and system write operations, which would otherwise cause sudden system crashes and unexpected downtime.




