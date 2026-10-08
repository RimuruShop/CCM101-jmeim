# Reflection

### 1. Why is object storage better suited for storing millions of photos compared to a traditional block storage hard drive?

Block storage works like a regular hard drive connected to a virtual machine. It is useful for applications that need fast and organized data access, but it is not ideal for handling millions of unstructured files. Object storage is designed to store large amounts of data using scalable buckets, where each file is stored as an object with its own ID and metadata. This makes object storage more suitable for millions of photos because the files can be easily stored and accessed without relying on a traditional file system.

### 2. How did using Docker make it easier to deploy the MinIO storage server?

Docker made the deployment process much easier because I did not have to manually install MinIO, configure its dependencies, or set up the network separately. With just one Docker command, I was able to run a working MinIO storage server. The `-e` flags were used to configure the login credentials, while the `-p` flags allowed the necessary ports to be accessed. Everything was contained in one easy-to-manage Docker container.

### 3. What is a "bucket" in the context of cloud storage?

A bucket is a main storage container used in object storage to hold files or objects. It is different from a normal folder because object storage does not depend on a traditional folder hierarchy. Instead, objects are stored inside the bucket and can be identified using their unique names or IDs.

### 4. How do you think large enterprise companies ensure their object storage data is not lost if the physical server crashes?

Large companies protect their data by creating multiple copies and storing them across different drives, servers, or locations. This process is called data replication and helps prevent data loss when hardware fails. Companies also use regular backups as an additional layer of protection. This is important because replication by itself may also copy accidentally deleted or corrupted data.

### 5. How is your confidence in navigating the Linux command line growing?

After completing five laboratory activities, I feel more comfortable using the Linux command line. Running Docker commands and managing containers through the terminal now feels more natural compared to Lab 1, when I was still learning basic commands such as `ls` and `cd`. Being able to deploy a working storage server using just one command has also helped me become more confident. The terminal is starting to feel less intimidating and more like a useful tool for completing different cloud computing tasks.
