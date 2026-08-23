**Compute Resources**
**Purpose:** Supplies the processing power (CPU and RAM) needed to run applications and workloads.
**Importance in cloud computing:** Compute is one of the main resources provided by cloud platforms. It executes programs, hosts applications, and handles data processing (e.g., EC2, Azure VMs, Compute Engine).
**In this environment:** The KillerCoda VM serves as the compute resource. Its CPU cores and RAM, identified in Checkpoint 2, determine the processing capacity available for running services.

**Storage Resources**
**Purpose:** Stores and maintains data such as files, databases, and system logs separately from the compute resources.
**Importance in cloud computing:** Cloud storage is designed to provide reliable, scalable, and persistent data storage, even when a compute instance is removed or restarted.
**In this environment:** The disks and mounted filesystems displayed using `df -h` represent the storage resources connected to the KillerCoda instance.

**Networking Resources**
**Purpose:** Allows compute and storage resources to communicate with each other and connect to external networks such as the internet.
**Importance in cloud computing:** Networking enables communication between services, controls access through security features such as firewalls and VPCs, and allows applications to be accessed remotely.
**In this environment:** The VM's IP address and hostname identify it within the network, similar to how a cloud-based virtual machine uses private or public IP addresses within a VPC.

**Operating System**
**Purpose:** Controls the system's hardware resources and provides the environment needed for applications and services to operate.
**Importance in cloud computing:** Most cloud computing services use operating systems, with Linux being widely used because of its efficiency, flexibility, and open-source nature.
**In this environment:** The Linux distribution and kernel version identified in Checkpoint 2 represent the operating system layer running on the KillerCoda compute instance.
