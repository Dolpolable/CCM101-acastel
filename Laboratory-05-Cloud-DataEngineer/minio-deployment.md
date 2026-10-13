# MinIO Object Storage Deployment Documentation

## 1. Deployment Command
The MinIO object storage server was deployed as a detached Docker container using the following command:

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server \
  -e "MINIO_ROOT_USER=cloudadmin" \
  -e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
  minio/minio server /data --console-address ":9001"
```
 ## 2. Port Configuration
Web Console Port: 9001 (mapped via -p 9001:9001 and specified with --console-address ":9001")

S3 API Port: 9000 (mapped via -p 9000:9000)

 ## 3. Bucket Details
Bucket Name: cloudnova-assets (or replace with the exact bucket name created in your web console, e.g., cloudnova-storage)

 ## 4. Environment Variables (-e Flags)
The -e flags pass environment variables into the runtime environment of the container prior to execution:

-e "MINIO_ROOT_USER=cloudadmin": Defines the administrative root username for the MinIO instance.

-e "MINIO_ROOT_PASSWORD=CloudNova2026!": Sets the root password required for authentication.

These variables configure the initial authentication credentials needed to access both the MinIO Web Console and the S3-compatible REST API endpoints.
