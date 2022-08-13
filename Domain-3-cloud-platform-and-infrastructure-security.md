# Cloud platform and infrastructure security

**Domain 3 topics**

- Disaster recovery
- Cloud infrastructure
- Secure cloud data center
- Risks to cloud infrastructure
- Counter-measures
- Business continuity

**Module reflection**

- What cloud infrastructure are you responsible for protecting?

- How familiar are you with your organizations business continuity process?

- What is your disaster recovery process?

---

## Cloud infrastructure components

**Components**

![plot](./imgs/03_01_cloud_components.png)

**Shared responsibility model**

![plot](./imgs/03_02_shared_responsibility_model.png)

**Quiz Question**

Infrastructure security is the responsibility of the hosting provider?

- True
- False
- Mostly true, Correct

---

## The management plane

The management or control plane is really the central way that hardware, logical and network configurations are administered and deployed throughout the cloud environment (e.g. new hardware spin up, routing traffic, data flow)

**Management plane**

- Physical
- Logical
- Networking

**Control plane**

- How data moves

**Data or forwarding plane**

- Receive and forward traffic

there should be redundancy and strong access control when it comes to implementing and managing aspects through the management plane.

**Module reflection**

- How is access to your organization's management plane managed?

- How do you ensure that the management plane is configured correctly?

- How do you ensure that sufficient redundancy is in place?

---

## Administering middleware

Middleware is software that access a bridge between the OS or DB or applications especially on the network

Specially important to PaaS and SaaS

**Shared administration of middleware**

- Secure OS baseline
  - Difficulty patching images
  - in a cloud environment, in a VM the OS is on a file and can't be patched. You should ensure that whenever a virtual environment is activated there is a configuration check to ensure that it is up to date with the most appropriate security configurations and patches
- Secure application
  - Configuration templates
- Middleware
  - Version control
  - Change management
  - Third-party licenses

**Quiz Question**

Which of the following is not true about virtual images?

- Virtual images provide a solution for backing up customer OS and configurations
- Virtual images restoration needs to be test regularly to ensure that it worked
- Virtual images can be patched easily because the data is compressed, Correct

---
