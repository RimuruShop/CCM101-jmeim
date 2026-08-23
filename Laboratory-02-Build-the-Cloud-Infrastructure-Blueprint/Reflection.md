# Cloud Infrastructure Components

## Compute Resources

**Purpose:** Compute resources supply the processing power required to run applications, perform calculations, and support the operating system. They are commonly provided through virtual machines, containers, or serverless functions.

**Why it matters in cloud computing:** Compute is the foundation of cloud workloads because applications need processing power to function. Cloud providers allow organizations to increase CPU/RAM or add more virtual machines when needed, avoiding the cost of purchasing physical servers.

**Relation to KillerCoda:** The KillerCoda playground is a virtual machine that serves as a compute resource. It is provided on demand and gives me a complete Linux environment without requiring physical hardware.

## Storage Resources

**Purpose:** Storage resources provide space for keeping the operating system, application files, and other data. Cloud storage can be provided through object, block, or file storage.

**Why it matters in cloud computing:** Storage must be dependable, scalable, and accessible when needed. Cloud storage reduces the limitations of physical disks by distributing data across different systems to improve durability.

**Relation to KillerCoda:** The disk space displayed by `df -h` in my playground represents block storage connected to my virtual machine, similar to the root storage volume used by cloud VMs in AWS, Azure, or GCP.

## Networking Resources

**Purpose:** Networking resources enable communication between virtual machines, storage systems, cloud services, and users. These resources include virtual networks, routers, firewalls, and load balancers.

**Why it matters in cloud computing:** Networking allows separate compute and storage resources to communicate and enables users to access applications. Proper network configuration also helps protect systems from unauthorized access.

**Relation to KillerCoda:** My playground has its own hostname and IP address, which I identified using `hostname` and `hostname -I`. These represent how the playground connects within KillerCoda's underlying cloud infrastructure and allows me to access it remotely through my browser.

## Operating System

**Purpose:** The operating system manages hardware resources, runs applications, and provides the interface, such as the Linux terminal, that I use to interact with the machine.

**Why it matters in cloud computing:** Most cloud servers use Linux distributions because they are lightweight, stable, and widely supported. The operating system provides the environment where cloud engineers configure, secure, and manage other resources.

**Relation to KillerCoda:** My playground runs Ubuntu 24.04.4 LTS, which I confirmed using `cat /etc/os-release`. This is similar to the Linux distributions commonly installed on cloud virtual machines such as AWS EC2, Azure VMs, and Google Compute Engine.

