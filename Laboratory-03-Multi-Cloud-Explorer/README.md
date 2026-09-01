Laboratory 03 — Multi-Cloud Explorer

🎯 Mission
This laboratory focuses on exploring three major cloud platforms: **Amazon Web Services (AWS), Microsoft Azure, and Google Cloud Platform (GCP)**. The goal is to examine their services, compare their capabilities, and determine which platform is appropriate for different business needs as part of the CloudNova Technologies Cloud Evaluation Team.


📂 Contents
| File                              | Description                                                 |
| --------------------------------- | ----------------------------------------------------------- |
| 🟠 `aws-research.md`              | Information and research about Amazon Web Services          |
| 🔵 `azure-research.md`            | Information and research about Microsoft Azure              |
| 🔴 `gcp-research.md`              | Information and research about Google Cloud Platform        |
| ⚖️ `cloud-platform-comparison.md` | Comparison of AWS, Azure, and GCP and service matching      |
| 🧭 `client-recommendations.md`    | Recommended cloud platforms for different client situations |
| 📄 `README.md`                    | Laboratory overview and Linux server investigation          |


🐧 Linux Investigation — Checkpoint 7
For this checkpoint, I used a *KillerCoda Playground** to examine a Linux virtual server. Several Linux commands were executed to identify the operating system, processor, memory, and available disk space.

🔍 System Information
| Information      | Command Used | Result                                                              |
| ---------------- | ------------ | ------------------------------------------------------------------- |
| Operating System | `uname -a`   | Ubuntu Linux 6.8.0-138-generic, x86_64 architecture                 |
| CPU              | `lscpu`      | Intel Xeon E312xx (Sandy Bridge), 1 CPU and 1 core, KVM virtualized |
| Memory           | `free -h`    | 1.9 GiB total, 416 MiB used, 854 MiB free, 1.5 GiB available        |
| Disk Space       | `df -h`      | `/dev/vda1` has 19 GB total, 5.4 GB used, and 13 GB available       |

📸 Terminal Screenshot
<img width="1366" height="1368" alt="ffff" src="https://github.com/user-attachments/assets/94fafb5c-95a7-423f-a0f5-9a6011876518" />






☁️ Cloud Migration of the Linux Server

The Linux server can be transferred to a cloud environment because all three cloud providers support Ubuntu-based virtual machines. The server has relatively small resource requirements, so a basic cloud virtual machine would be sufficient for a similar workload.

| Cloud Provider | Possible Service           | Purpose                               |
| -------------- | -------------------------- | ------------------------------------- |
| 🟠 AWS         | Amazon EC2                 | Runs the Ubuntu Linux virtual machine |
| 🔵 Azure       | Azure Virtual Machines     | Provides a cloud-based Linux server   |
| 🔴 GCP         | Google Compute Engine      | Hosts the Linux virtual machine       |

Explanation
If this server were moved to the cloud, Amazon EC2, Azure Virtual Machines, or Google Compute Engine could be used to host it. These services allow users to select a Linux operating system and assign computing resources based on the workload.
For this particular server, a small virtual machine would be a practical starting point because it only has one CPU core, around 2 GiB of memory, and a 19 GB disk. If the server becomes busier, additional CPU, memory, or storage can be assigned later.
This shows that the same Linux workload can be supported by different cloud providers. The final choice would depend on factors such as price, available services, performance, security features, and the organization's requirements.
