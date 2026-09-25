# Mission 4: The Cloud-Native Engineer

> **Laboratory Activity 4** — CloudNova Technologies Cloud-Native Engineering Team

---

## 📋 Mission Overview

This laboratory activity focused on learning how modern cloud-native applications use containers instead of relying only on traditional virtual machines. Using the KillerCoda Playground, I explored the differences between Virtual Machines and Containers, practiced basic Docker commands, and deployed an Nginx web server inside a Docker container. The activity also helped me understand how containers can be created, accessed, managed, stopped, and removed.

---

## 🎯 Objectives

* ✅ Understand the main differences between Virtual Machines and Containers
* ✅ Use a cloud-based Linux environment through KillerCoda
* ✅ Practice essential Docker commands
* ✅ Download and deploy an Nginx container
* ✅ Test a containerized web server using a local port
* ✅ Manage the complete lifecycle of a Docker container
* ✅ Document the laboratory activity using Markdown

---

## 💻 Docker Commands Executed

| **Command**                                      | **Purpose**                                                  |
| ------------------------------------------------ | ------------------------------------------------------------ |
| `docker --version`                               | Displayed the installed Docker version                       |
| `docker info`                                    | Checked information and details about the Docker environment |
| `docker pull nginx`                              | Retrieved the Nginx image from Docker Hub                    |
| `docker run -d -p 8080:80 --name my-nginx nginx` | Created and started an Nginx container with port forwarding  |
| `curl http://localhost:8080`                     | Tested whether the Nginx web server was accessible           |
| `docker ps`                                      | Displayed the containers that were currently running         |
| `docker stop my-nginx`                           | Stopped the Nginx container                                  |
| `docker ps -a`                                   | Displayed all containers, including stopped containers       |
| `docker rm my-nginx`                             | Deleted the Nginx container from the system                  |

---

## 🧠 Skills Learned

Through this activity, I learned how Virtual Machines and Containers differ in terms of architecture and resource usage. I also gained practical experience using Docker in a Linux environment.

The activity helped me practice:

* Identifying the differences between a VM and a container
* Checking Docker installation and system information
* Downloading images from Docker Hub
* Creating and running containers
* Using detached mode to run a container in the background
* Understanding host and container port mapping
* Testing a running web service using `curl`
* Viewing, stopping, and removing Docker containers
* Organizing technical information using Markdow
