# Cloud Infrastructure Components Identification

## 1. Compute Resources
* **Purpose:** Provides processing power and memory execution environments needed to run applications and process data.
* **Importance in Cloud:** Allows systems to dynamically scale CPU and RAM on demand to handle varying workloads without physical hardware upgrades.
* **Relation to KillerCoda Environment:** Represented by the virtualized CPU cores (`lscpu`) and RAM allocations (`free -h`) assigned to our KillerCoda container instance.

## 2. Storage Resources
* **Purpose:** Offers non-volatile data retention for operating systems, application files, user data, and databases.
* **Importance in Cloud:** Ensures data persistence, back-up resilience, and access across distributed systems through block, object, or file storage solutions.
* **Relation to KillerCoda Environment:** Observed via root block storage partitions and virtual file systems mounted at `/` using the `df -h` command.

## 3. Networking Resources
* **Purpose:** Facilitates data communication between instances, external networks, users, and cloud services.
* **Importance in Cloud:** Enables secure connectivity, routing, load balancing, and network isolation using Virtual Private Clouds (VPCs).
* **Relation to KillerCoda Environment:** Demonstrated by the system hostname and local/private IP addresses assigned to virtual network interfaces viewed via `ip a`.

## 4. Operating System
* **Purpose:** Acts as the interface between system software/applications and the underlying physical or virtualized hardware resources.
* **Importance in Cloud:** Delivers the environment, libraries, and security controls needed to deploy and run cloud software seamlessly.
* **Relation to KillerCoda Environment:** Represented by the Ubuntu Linux distribution (`cat /etc/os-release`) and Linux kernel (`uname -r`) powering the server instance.
