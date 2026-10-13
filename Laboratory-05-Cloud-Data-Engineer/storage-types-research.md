# Research: Types of Cloud Storage #


| **Storage Type** | **Description (How it stores data)** | **Primary Use Case (Best used for)** | **Cloud Provider Example** |
|----|----|----|----|
| **Block Storage** | Raw storage volumes broken into fixed-size blocks; attached as drives to OS. | High-performance databases, boot volumes, and transactional workloads. | AWS EBS (Elastic Block Store) |
| **File Storage** | Data stored as a hierarchy of files and folders within a shared directory structure. | Collaborative file sharing, network-attached home directories, and NAS.| AWS EFS (Elastic File System) |
| **Object Storage** | Data managed as distinct units (objects) with metadata and unique identifiers in a flat flat namespace. | Storing massive amounts of unstructured data like backups, media, and user uploads. | AWS S3 (Simple Storage Service) | 

## Explainaation why Object Storage s the best choice for storing their user-uploaded images. ##
Object storage is the optimal choice for your photo-sharing application because it scales infinitely, handles massive amounts of unstructured media files natively, and makes each image easily accessible via web APIs. Unlike block storage, it is designed specifically to cost-effectively store millions of independent files without being bound to a single virtual server's file system.
