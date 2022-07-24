# Domain 1: Cloud Concepts, Architecture, and Design

## Essential Characteristics

What enables cloud computing

- Broad Network Access
  - Internet connection to connect remotely to someone else's server on the cloud
- Rapid Elasticity
  - Easily scale up and scale down architectures
- Measured / Metered Service
  - only pay for what you use
- On-Demand Self-Service
  - always access and provision resources in the cloud
- Resource Pooling
  - shared resources are really what enable and make cloud computing cost benefit many companies

## Service Models

- SaaS (Software as a Service)
  - applications that are based in the cloud (Microsoft Office, G suite etc)
- PaaS (Platform as a Service)
  - spinning up development environments and developing new applications and software
- IaaS (Infrastructure as a Service)
  - e.g. having your own hardware stored in a Data center or being able to select your operating system and installing on hardware, hosted in someone else's data center

## Deployment Models

- Public
  - probably the most economical, but there isn't much control in terms of the shared resources, data security
- Private
  - most control, with greatest expense
- Hybrid
  - mix of any of the other 3 models
- Community
  - managed by de-centralized organizations or one organization that utilizes cloud resources

> The business case for why you are using the cloud either as a service or as a deployment method drives the security and the concerns on how you are going to secure your cloud environment

---

> "Cloud Computing is a model for enabling ubiquitous, convenient, on-demand network access to a shared pool of configurable computing resources (e.g., networks, servers, storage, applications, and services) that can be rapidly provisioned and released with minimal management effort or service provider interaction."

NIST 800-154 Cloud Computing Definition

---

## What are the different roles in cloud computing?

- Customer
  - the person or the organization that is purchasing services from a Cloud Provider
- Cloud Service Provider (CSP) or Cloud Provider
  - is the organization that actually provides the psychical infrastructure that is being accessed through the internet. Major providers include AWS, Microsoft Azure, Google Cloud
- Cloud Broker
  - negotiates with the Cloud Service Provider on behalf of the customer as well as may deploy their own service to help the customer manage and get the most out of their cloud deployment
  - optimization features
- Cloud Access Security Broker (CASB)
  - application or server itself that sits between the customer and access portal to it's cloud hosted applications or server. It's role is to enforce the access logging policies for the organization.
  - identity and access management, enforcing the organization security policies to securely monitor activity in the cloud

**Quiz Question**

Which role is paid to monitor access and enforce security policies for cloud environments?

- Customer
- Cloud broker
- Cloud access security broker (CASB): Correct

---

## Cloud Security Concepts

**Security Principles**

- Confidentiality
  - ensuring that only those people who need access to the cloud, have access to it.
- Integrity
  - ensuring that no modification can be made to data or apps without proper monitoring
- Availability
  - access the cloud instance

**Security Process**

- Data security
  - The risc associated with protecting the data really dictates what counter measures you employ in the cloud to keep that data safe
- Virtualization
  - Although there are physical servers that you utilize in the cloud, there are also virtual servers. Cloud computing utilizes virtual servers and virtualization in order to augment the abilities of organizations. Virtual servers and virtualization have a number of configurations that need to be taken into consideration.
- Encryption
  - The process of applying algorithms to information to render them unable to be deciphered or read by unauthorized parties
- Auditing and Compliance
  - Ensure that everything that happens in the cloud, meets the legal guidelines applicable to your cloud, the data that you utilizing and customers that you have

**Quiz Question**

What aspect of the CIA triad is most important in the Cloud context?

- Availability: Correct
- Confidential
- Integrity

Without availability, there is nothing else.

---

## What are the Cloud Service models?

### Infrastructure as a Service (IaaS)

- Most control
- Most security responsibility

Cloud customer can choose the OS and hardware

Cloud Provider is accountable for the facilities, maintaining hardware, ensuring redundancy with the utilities, devices are patched

### Platform as a Service (PaaS)

- More control
- More security responsibility

Cloud customer is responsible of provisioning all the virtual environments, ensuring they are configured properly

Cloud provider maintains the operating system

### Software as a Service (SaaS)

- Least control
- Least security responsibility

If you are the cloud customer, you only need to make sure data and application is secure.

If you are providing the SaaS, you have to ensure the application is patched properly, APIs are maintained securely, secure connections, no back doors or flaws

- IaaS

  - APIs
  - Core Connectivity & Delivery
  - Abstraction
  - Hardware
  - Facilities

- PaaS = Iaas features plus

  - Integration & Middleware

- SaaS = PaaS plus
  - Presentation Modality
  - Presentation Platform
  - APIs
  - Applications
  - Data
  - Metadata
  - Content

**Quiz Question**

Which service model provides the greatest control as well as responsibility for security?

- Infrastructure as a Service (IaaS) Correct
- Software as a Service (SaaS)
- Platform as a Service (PaaS)
