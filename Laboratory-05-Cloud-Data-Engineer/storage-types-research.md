# Cloud Storage Architecture Research

> **Theoretical Analysis:** A study of the three major cloud storage approaches and their appropriate uses in modern applications.

---

##  Comparison Matrix

| **Storage Type**       | **How It Works**                                                                                            | **Common Uses**                                                                                     | **AWS Example**                     |
| ---------------------- | ----------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- | ----------------------------------- |
| ** Block Storage**   | Stores information as individual blocks that can be formatted and managed by an operating system.           | Virtual machine disks, operating systems, and databases that require fast data access               | **AWS EBS** (Elastic Block Store)   |
| ** File Storage**    | Organizes information using a familiar folder and file structure that can be accessed through a network.    | Shared folders, content management systems, and applications that require a traditional file system | **AWS EFS** (Elastic File System)   |
| ** Object Storage** | Stores files as objects together with metadata and a unique identifier, which can be accessed through APIs. | Photos, videos, backups, static website files, and large collections of unstructured data           | **AWS S3** (Simple Storage Service) |

---

##  Architectural Recommendation

>  **Client Advisory Note:** *Recommended Storage Approach for User-Generated Content*

### Why Object Storage Is Suitable for User-Uploaded Images

For an application that needs to store a large number of user-uploaded images, **Object Storage** is a practical choice. It is designed to handle large amounts of unstructured data and can scale as the number of files increases.

Unlike block storage, which is commonly used for virtual disks and databases, or file storage, which follows a traditional folder structure, object storage keeps each file as an individual object. Each object can also contain metadata that provides additional information about the file.

Object storage can also be accessed through HTTP-based APIs, making it convenient for web and mobile applications. For example, an application can upload an image to a storage bucket and later retrieve it when the user needs to view it.

Overall, object storage provides a flexible way to manage user-generated images while supporting scalability, metadata, API-based access, and integration with modern cloud applications.
