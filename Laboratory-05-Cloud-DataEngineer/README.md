---

### `README.md` (Laboratory-05-Cloud-Data-Engineer)

```markdown
# Laboratory 05: Cloud Data Engineer

## Mission Overview
This laboratory covers the fundamental concepts of cloud storage architectures and the practical deployment of an on-premises, S3-compatible object storage infrastructure. The mission involves analyzing the differences between Block, File, and Object storage, deploying an isolated MinIO server container via Docker on Linux, managing network ports and environment variables, and configuring storage buckets through a web-based management console.

## Objectives
* Analyze and compare the three primary cloud storage architectures: Block Storage, File Storage, and Object Storage.
* Deploy an S3-compatible MinIO object storage container using Docker CLI.
* Configure runtime container settings using environment variables and port forwarding.
* Access the MinIO Web Console and manage storage buckets and access policies.
* Document technical deployment processes and configuration specifications.

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
