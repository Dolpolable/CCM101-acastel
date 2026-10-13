# Checkpoint 2 - Research: Types of Cloud Storage

## Cloud Storage Comparison

| Storage Type | Description (How does it store data?) | Primary Use Case (What is it best used for?) | Cloud Provider Examples |
| :--- | :--- | :--- | :--- |
| **Block Storage** | Splitting data into raw, fixed-sized chunks called "blocks," each with a unique identifier but without metadata. Blocks are presented directly to an OS as a raw disk volume. | Transactional databases, OS boot drives, virtual machine disks, and applications requiring ultra-low latency and granular read/write access. | • AWS Elastic Block Store (EBS)<br>• Azure Managed Disks<br>• Google Cloud Persistent Disk |
| **File Storage** | Organizing data hierarchically in a directory tree consisting of folders, subfolders, and files, accessed via standard network sharing protocols (NFS/SMB). | Shared application files, content management systems (CMS), legacy system migrations, and team collaboration shares requiring simultaneous multi-user access. | • AWS Elastic File System (EFS)<br>• Azure Files<br>• Google Cloud Filestore |
| **Object Storage** | Storing data as self-contained discrete units ("objects") in a flat address space, combining the file data, rich customizable metadata, and a globally unique identifier accessible via HTTP REST APIs. | Unstructured data repositories, static web asset hosting, media streaming libraries, backups, archives, and massive big-data analytics lakes. | • AWS Simple Storage Service (S3)<br>• Azure Blob Storage<br>• Google Cloud Storage |

---

## Client Recommendation: Why Object Storage?

Object Storage is the ideal solution for your use case because it delivers virtually unlimited horizontal scalability and industry-leading durability at a fraction of the cost of block or file systems. Its flat architecture pairs files with rich, customizable metadata, making massive collections of unstructured media and documents easily indexable, secure, and globally accessible over standard web protocols (HTTP/HTTPS). This allows your application to scale seamlessly to petabytes of data without managing underlying drive partitions or running into file system hierarchy bottlenecks.
