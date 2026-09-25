# Technical Documentation: MinIO Container Deployment

---

## 🚀 Docker Execution Command

To set up the MinIO object storage service, I created a Docker container and configured it to provide both an S3-compatible API and a web-based management console. The following command was used to deploy the MinIO server:

```bash
docker run -d \
  -p 9000:9000 \
  -p 9001:9001 \
  --name minio-server \
  -e "MINIO_ROOT_USER=cloudadmin" \
  -e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
  minio/minio server /data --console-address ":9001"
```

### Command Explanation

| **Option / Command**                    | **Purpose**                                             |
| --------------------------------------- | ------------------------------------------------------- |
| `docker run -d`                         | Creates and starts the container in detached mode       |
| `-p 9000:9000`                          | Connects host port 9000 to MinIO's API port             |
| `-p 9001:9001`                          | Connects host port 9001 to the MinIO web console        |
| `--name minio-server`                   | Assigns the container the name `minio-server`           |
| `-e MINIO_ROOT_USER=cloudadmin`         | Sets the administrator username                         |
| `-e MINIO_ROOT_PASSWORD=CloudNova2026!` | Sets the administrator password                         |
| `minio/minio`                           | Specifies the MinIO Docker image                        |
| `server /data`                          | Starts MinIO and uses `/data` as its storage directory  |
| `--console-address ":9001"`             | Configures the MinIO web console to listen on port 9001 |

### Deployment Result

After executing the command, the MinIO container starts in the background. Port **9000** is available for S3-compatible API requests, while port **9001** is used to access the MinIO web interface. This configuration allows files and other objects to be managed through the MinIO console while also supporting applications that communicate using the S3 API.

> **Note:** In an actual production environment, administrator credentials should be stored securely rather than written directly in command history or documentation.
