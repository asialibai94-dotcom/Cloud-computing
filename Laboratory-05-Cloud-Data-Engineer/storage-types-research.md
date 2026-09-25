# Storage Types Research

## Comparison of Cloud Storage Types

| Storage Type | Description | Primary Use Case | Cloud Provider Example |
|---|---|---|---|
| Block Storage | Stores data in fixed-size blocks that can be accessed individually. It behaves like a virtual hard drive attached to a computer or server. | Best for operating systems, databases, and applications that need fast and direct access to storage. | AWS EBS |
| File Storage | Stores data as files inside folders and directories. Multiple users or systems can access the same file system over a network. | Best for shared files, documents, media files, and applications that need a shared file system. | AWS EFS |
| Object Storage | Stores data as objects together with metadata and a unique identifier. Objects are stored inside containers called buckets. | Best for large amounts of unstructured data such as images, videos, backups, and documents. | AWS S3 |

## Why Object Storage is Suitable for the Client

Object Storage is a good choice for the client's photo-sharing application because it is designed to store large amounts of unstructured data such as images. It can also scale to handle millions of files while keeping the data accessible through applications and web services.
