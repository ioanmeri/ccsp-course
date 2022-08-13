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

## Virtualization

The ability to create environments in the cloud that individual customers can utilize, take advantage of shared resources.

- Hypervisor hardening
  - logging & monitoring
  - updated & patched
  - Hypervisor (I & II)
    - I is more safe as each one of the virtual machines have their own OS
- Instance Isolation
  - logical isolation
    - for software and digital assets, is applied at the instance level. Each VM is logically protected from communicating with another VM
  - prevents data leakage and inter-vm attacks
  - Sandbox testing
- Host Isolation
  - Physical & logical isolation
  - Monitor for guest escape

**Hypervisor types 1 and 2**

![plot](./imgs/03_03_hypervisor_types.png)

**Quiz Question**

What type of attack is characterized by a user on a virtual instance attempting to elevate themselves to leave the VM and access the network?

- Guest escape, Correct
- Inter-VM attack
- Logical isolation

---

## Data access

The customer is always responsible for protecting the data in the theoretical and legal sense.

**Data access administration**

- Customer access administration
- Provider access administration
- Cloud access security broker (CASB)

**Module reflection**

- How many groups need access to your cloud environments?

- How could the administration of cloud data access at your organization been improved?

---

## Secure networking

**Maintaining a secure network**

- Virtual local area networks (VLAN)
  - a way of ensuring there is logical separation between VMs / networks on physical hardware
- Dynamic host configuration protocol (DHCP)
  - assigns an IP address to a device, enables routing, for a specific period of time so the IP can be re assigned
- Domain Name Service (DNS)
  - Configuration
  - Maintenance
  - DNS poisoning attack, attackers will change entries in the DNS table to disguise the origin of their attack
- Virtual private network (VPN)
  - encrypting tunnel between end points

**Quiz Question**

Which of the following is used to isolate network segments and prevents an attacker from moving through the network?

- DNS
- VLAN, Correct
- DHCP

---

## Network Security

**Cloud provider responsibility for network security**

- Protection
  - Firewall administration
- Detection
  - IDS (Intrusion detection system) /IPS (Intrusion prevention system)
  - Honeypot
    - intentionally setup to appear valuable or vulnerable systems that attract would-be attackers to investigate them. Honeypot registers the signature of the attacker and alerts the company.
- Communication protection
  - Virtual private network
  - Encryption
  - Strong authentication
- Improvement
  - Vulnerability assessments

**Quiz Question**

What is the key difference between IDS and IPS?

- An IDS uses analysis of behavior and an IPS uses a defined rule set

- An IDS actively closes port and services upon detection but and IPS prevent attackers from entering the network

- An IDS only reports suspicious activity and an IPS also takes defensive action, Correct

---

## System information and Event Management (SIEM)

**Security improvements of a SIEM:**

- Centralizes logging
- Enhanced analysis
- Dashboards and visualizations
- Automated response

Unless you have proper asset management to understand what needs to be monitored, it can be difficult to get values out of the SIEM.

That's why business impact analysis is critical for SIEM to function properly.

(e.g. anomalies logging of IP addresses outside the location employees working from)

**Quiz Question**

Which of the following is most important for effective SIEM operations?

- Asset management, Correct
- Alert optimization
- Incident response

---

## Cloud provider responsibility for physical plant

**Responsibilities include**

- Physical location
  - not in highly populated, or very remote (not many business and staff), political situation
- Secure and manage hardware components
- Log events and incidents
- Configure secure remote administrative access

**Quiz Question**

Which of the following dictates how processors can be used for cryptographic functions?

- Trusted Platform Module (TPM)
- Hardware controller
- Advanced Encryption Standard (AES)

---

## Power redundancy

**Physical environment**

- Availability
  - 99,999% up time, 6 minutes down time / yr
- Power
  - Data center and components
  - HVAC
  - Lighting
- Accidental power loss
- Conditioning
  - Uninterruptible power supply (UPS)

**Quiz Question**

How much unscheduled downtime is allowed by the five nines availability standard?

- 60 minutes
- 30 minutes
- 6 minutes, Correct

---
