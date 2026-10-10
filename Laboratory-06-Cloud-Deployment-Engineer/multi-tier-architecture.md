# Two-Tier Architecture

## Introduction
A Two-Tier Architecture is a system design that separates an application into two main parts: the Web/Application Tier and the Database Tier. These tiers communicate with each other to provide services to users.

## 1. The Web/Application Tier
The Web/Application Tier handles user requests and displays the application's user interface. In this project, Nextcloud serves as the web application. It receives HTTP requests through port 8080 and communicates with the database when information needs to be stored or retrieved.

## 2. The Database Tier
The Database Tier stores and manages persistent application data, such as user accounts, settings, and other database records. In this project, MariaDB stores the information used by Nextcloud. The database runs in a separate container named `database`.

## 3. Why Separate Them?
Separating the web application and database into different containers makes the system easier to maintain, troubleshoot, and update. Each container can be managed independently, and resources can be allocated according to its needs. This separation also helps organize the application, although additional security controls and network configuration are still needed to protect the database.

## Conclusion
The two-tier architecture used in this mission demonstrates how Docker Compose connects separate services to create a functioning cloud application.
