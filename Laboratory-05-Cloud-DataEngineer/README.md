---

### `README.md` (Laboratory-05-Cloud-Data-Engineer)

```markdown
# Laboratory 05: Cloud Data Engineer

## Mission Overview
Congratulations! Your seamless deployment of containerized web servers has caught the attention of
the senior architects. You have now been temporarily reassigned to the Cloud Data Engineering Team at
CloudNova Technologies.
In the cloud, data is everything. However, not all data is stored the same way. While traditional
computers use hard drives (Block Storage) and shared network drives (File Storage), modern cloud applications
rely heavily on Object Storage to store massive amounts of unstructured data like images, videos, and backups.
The industry standard for this is Amazon S3, but today, you will deploy your very own S3-compatible cloud
storage server using an open-source tool called MinIO.
Using your KillerCoda Playground, you will combine your new Docker skills with your cloud storage knowledge to
deploy a live object storage server, create a storage "bucket," and upload data over the web.
Remember: A cloud engineer doesn't just store data; they ensure it is scalable, accessible, and secure.

## Objectives
At the end of this laboratory activity, you should be able to:
 Differentiate between Block, File, and Object Storage.
 Deploy an S3-compatible Object Storage server (MinIO) using Docker.
 Access a cloud service via a web interface using port forwarding.
 Create a storage bucket and upload objects (files) to the cloud.
 Document cloud storage operations using Markdown.
 Continue expanding a professional GitHub Cloud Computing Portfolio.

## Tools Used
* **Operating System:** Ubuntu Linux (KillerCoda Playground)
* **Container Engine:** Docker Engine / Docker CLI
* **Object Storage Server:** MinIO (`minio/minio`)
* **Protocols & Interfaces:** S3 API (Port 9000), HTTP Web Console (Port 9001)
* **Documentation:** Markdown

## Skills Learned
* **Storage Architecture Evaluation:** Differentiating data persistence models based on latency, structure, scalability, and application use cases.
* **Containerized Service Deployment:** Running multi-port containerized services with persistent storage paths in detached mode.
* **Security & Credential Management:** Supplying root credentials securely through runtime environment variables (`-e`).
* **Object Storage Operations:** Creating and managing buckets, handling object uploads, and navigating S3-compatible web management interfaces.
