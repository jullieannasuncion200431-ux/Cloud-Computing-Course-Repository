# Laboratory Activity 5: The Cloud Data Engineer

> **Laboratory Activity 5** — CloudNova Technologies Cloud Data Engineering Team

---

## 📌 Mission Overview

This laboratory activity focused on understanding how cloud-based object storage can be used to store and manage files separately from application containers. As part of the Cloud Data Engineering Team at **CloudNova Technologies**, I used Docker and MinIO to create an S3-compatible storage environment.

The activity demonstrated how MinIO can provide a reliable location for storing unstructured files such as images, documents, and other media. By separating the storage system from the application container, files can remain available even when containers are restarted or replaced.

---

## 🎯 Objectives & Key Deliverables

The main objectives of this laboratory activity were:

* **Storage Research:** Learn the differences between Block Storage, File Storage, and Object Storage.
* **MinIO Deployment:** Set up a MinIO server using Docker.
* **Docker Configuration:** Use environment variables and port mapping when creating the container.
* **Web Access:** Access the MinIO management console through a web browser.
* **Bucket Creation:** Create a storage bucket named `client-photos`.
* **Object Management:** Upload and manage files inside the created bucket.
* **Documentation:** Record the procedures, commands, and observations in Markdown format.

---

## 🛠️ Stack & Infrastructure

| **Component**          | **Technology**        | **Purpose**                                                 |
| ---------------------- | --------------------- | ----------------------------------------------------------- |
| **Container Platform** | Docker                | Used to run the MinIO service in an isolated container      |
| **Object Storage**     | MinIO                 | Provides S3-compatible storage for files and media          |
| **Operating System**   | Linux (Ubuntu)        | Provides the environment for running Docker                 |
| **Cloud Environment**  | KillerCoda Playground | Used as the temporary cloud-based laboratory environment    |
| **Web Console**        | Port 9001             | Used to access and manage MinIO through a browser           |
| **S3 API**             | Port 9000             | Provides access to MinIO through S3-compatible applications |

---

## 💡 Key Skills Learned

During this activity, I developed practical knowledge about cloud storage and containerized storage services.

### 🐳 Docker Configuration

I learned how to create and manage containers using Docker commands. I also practiced assigning ports and configuring environment variables when deploying MinIO.

### ☁️ Object Storage Management

I learned how object storage organizes files using buckets and objects. I also practiced creating a bucket and uploading files through the MinIO interface.

### 🔐 Storage Access

The activity helped me understand why storage services need controlled access and proper configuration when handling application data.

### 📡 S3 Compatibility

I learned that MinIO follows the S3 API standard, which allows applications designed to work with Amazon S3-compatible storage to communicate with MinIO.

### 📝 Technical Documentation

I also improved my ability to document commands, configurations, and results using Markdown so that the deployment process can be easily understood and repeated.

---

## ⚠️ Challenges Encountered

One of the challenges I encountered was understanding the purpose of the two MinIO ports. At first, I was confused about why the deployment required both **9000** and **9001**. After exploring the setup, I learned that port 9000 is mainly used for the S3-compatible API, while port 9001 provides access to the MinIO web console.

Another challenge was making sure that the Docker container was configured correctly, especially the environment variables and port mappings. A small mistake in the configuration could prevent MinIO from starting or make the web console inaccessible.

I also needed to carefully manage the KillerCoda session because the playground environment is temporary. I had to complete the deployment, create the bucket, upload the required files, and capture screenshots within the available session time.

Overall, this laboratory helped me understand how object storage can be separated from application containers. It also gave me practical experience with Docker, MinIO, buckets, objects,
