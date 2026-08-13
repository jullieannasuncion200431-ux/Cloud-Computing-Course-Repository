# Cloud Infrastructure Components

## Compute Resources

**Purpose:** Compute resources supply the processing capability required to run programs, execute commands, and manage different workloads. The CPU performs the calculations and instructions needed by applications and system processes.

**Importance in cloud computing:** Compute resources are essential because they allow cloud applications and services to operate. They determine how much processing workload a cloud system can handle and can be increased or decreased depending on the requirements of the application.

**Relation to KillerCoda environment:** In the KillerCoda environment, the compute resource is provided by a virtual CPU running the Ubuntu Linux operating system. The CPU is responsible for executing the commands entered in the terminal and running the system processes.

## Storage Resources

**Purpose:** Storage resources provide space for saving the operating system, applications, configurations, and other data. They allow information to remain available for the system to use when needed.

**Importance in cloud computing:** Storage is important because cloud applications need a reliable place to keep files and data. Cloud platforms provide different types of storage that can be selected based on capacity, performance, availability, and cost.

**Relation to KillerCoda environment:** The Linux server uses virtual disk storage for its operating system and files. The available disk space and mounted partitions can be examined using commands such as `df -h` and `findmnt`.

## Networking Resources

**Purpose:** Networking resources provide communication between the cloud server, users, and other systems. They include network interfaces, IP addresses, and connections used to transmit information.

**Importance in cloud computing:** Networking allows cloud services to communicate with users and with other cloud resources. A properly configured network is necessary for accessing applications, transferring data, and connecting different services.

**Relation to KillerCoda environment:** The KillerCoda Linux server has network interfaces that allow it to communicate within its cloud environment. The `ip a` command can be used to identify the available network interfaces and their assigned IP addresses.

## Operating System

**Purpose:** The operating system controls computer resources and provides the environment needed to run applications and system processes. It acts as an intermediary between the hardware and software.

**Importance in cloud computing:** An operating system provides the foundation for running cloud workloads. It manages CPU, memory, storage, processes, networking, and security while providing tools that administrators use to manage the server.

**Relation to KillerCoda environment:** The KillerCoda environment uses a Linux-based operating system, Ubuntu. The operating system can be identified using `cat /etc/os-release`, while the kernel version can be checked using `uname -r`. These components allow the virtual server to execute commands and manage its available resources.
