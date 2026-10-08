# Cloud Storage Types Research

| Storage Type | Description | Primary Use Case | Cloud Provider Example |
|---|---|---|---|
| **Block Storage** | Stores data in fixed-size blocks, with each block having its own identifier. It is provided to a virtual machine as a raw storage volume, while the operating system manages the formatting and file system. | Used for boot drives and high-performance tasks such as transactional databases that require fast and low-latency data access. | Amazon EBS, Azure Disk Storage, Google Persistent Disk |
| **File Storage** | Organizes data as files and folders in a hierarchical structure. It can be accessed over a network using protocols such as NFS or SMB. | Useful for shared folders that need to be accessed by multiple users or virtual machines, such as applications that require a shared network drive. | Amazon EFS, Azure Files, Google Cloud Filestore |
| **Object Storage** | Stores data as individual objects in a scalable storage space called a bucket. Each object contains its data, metadata, and a unique identifier and can be accessed through HTTP/HTTPS and APIs. | Best for large amounts of unstructured data, including photos, videos, backups, website files, and archives. | Amazon S3, Azure Blob Storage, Google Cloud Storage |

## Why Object Storage Is Best for the Client's Photos

For a photo-sharing application that may receive millions of uploaded images, **Object Storage** is the most suitable option. It can easily handle huge amounts of unstructured data without requiring complicated folder structures or file management. Unlike block storage, which is mainly designed for high-performance workloads and attached volumes, object storage can scale to very large amounts of data. It can also be accessed through HTTP/HTTPS and simple APIs, making it easy to connect with a web application. In addition, it is generally more cost-effective for storing large collections of photos that do not need to be changed frequently.
