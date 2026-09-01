#  Cloud Platform Recommendations

## Client A — Startup Company

**Recommended Platform:** Google Cloud Platform (GCP)

**Explanation:**
GCP is a suitable choice for the startup because the company has a small budget while expecting its application to gain more users over time. Cloud resources can be adjusted as the application grows, helping the company avoid paying for resources it does not currently need. GCP also provides managed services that can reduce the amount of server administration required from a small development team.

**Services to use:**

* **App Engine** — Used to host the application's backend while allowing the platform to handle much of the server management and scaling.
* **Firebase** — Provides useful mobile application features such as user authentication, databases, and notifications.
* **Cloud Storage** — Used to keep application files, images, and other user-uploaded content.

---

## Client B — University

**Recommended Platform:** Microsoft Azure

**Explanation:**
Azure is a good match for the university because its existing infrastructure already uses Microsoft technologies. Using Azure can make it easier to connect the university's current Windows Server, Microsoft 365, and Active Directory environment with cloud services. This can also reduce the need to completely replace the university's existing systems.

**Services to use:**

* **Azure Virtual Machines** — Can be used to move existing Windows Server applications and workloads into the cloud.
* **Microsoft Entra ID** — Helps manage student, teacher, and staff identities and control access to university resources.
* **Azure Virtual Desktop** — Provides students and employees with access to applications and virtual desktops from supported devices.

---

## Client C — AI Research Company

**Recommended Platform:** Google Cloud Platform (GCP)

**Explanation:**
GCP is recommended for the AI research company because the company needs powerful computing resources and specialized tools for artificial intelligence and machine learning. Google Cloud provides services that support the development, training, testing, and deployment of AI models. It also provides computing resources that can be equipped with GPUs or other accelerators for demanding workloads.

**Services to use:**

* **Vertex AI** — Provides tools for creating, training, evaluating, and deploying machine learning models.
* **Compute Engine** — Provides virtual machines that can be configured with GPUs or other resources for demanding AI workloads.
* **BigQuery** — Used to store and analyze large datasets that can be useful for research and machine learning projects.

---

## Client D — Global E-Commerce Company

**Recommended Platform:** Amazon Web Services (AWS)

**Explanation:**
AWS is a strong option for the global e-commerce company because an online store needs reliable services that can handle customers from different locations. The company may also experience sudden increases in traffic during promotions, holidays, or major sales. AWS provides services that can automatically adjust computing resources, distribute traffic, and deliver website content efficiently to users.

**Services to use:**

* **Amazon EC2 with Auto Scaling** — Runs the e-commerce application and can increase or decrease computing capacity based on demand.
* **Amazon RDS** — Provides a managed relational database for information such as orders, customers, products, and inventory.
* **Amazon CloudFront** — Delivers website content from locations closer to customers, helping improve loading speed for users in different regions.

---

# Multi-Cloud Decision Matrix

| Business Requirement    | Recommended Platform        | Justification                                                                                                                   |
| ----------------------- | --------------------------- | ------------------------------------------------------------------------------------------------------------------------------- |
| Startup Company         | Google Cloud Platform (GCP) | Provides flexible cloud services that can support a small company as its application and number of users increase.              |
| Enterprise Organization | Amazon Web Services (AWS)   | Offers a wide range of services that can be used to build and manage large business systems.                                    |
| Microsoft Environment   | Microsoft Azure             | Works well with Windows Server, Microsoft 365, and Microsoft identity technologies.                                             |
| AI / Machine Learning   | Google Cloud Platform (GCP) | Provides specialized AI and machine learning services together with powerful computing and data tools.                          |
| Kubernetes Deployment   | Google Cloud Platform (GCP) | Google Cloud provides Google Kubernetes Engine (GKE), a managed service for running containerized applications with Kubernetes. |
| Global Web Application  | Amazon Web Services (AWS)   | Provides scalable infrastructure and global services that can support applications serving users from different locations.      |
