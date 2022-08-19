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

---

## Infrastructure as a Service (IaaS)

Customers can have any OS they want.

The hosting provider maintains:

- APIs
- Core Connectivity & Delivery
- Abstraction
- Hardware
- Facilities

and it's responsible for:

- Hardware
- Blades
- Facilities, Utilities, Connectivity, Physical security

Customers can use their backups to restore the production environments fairly quickly

**Drawbacks of IaaS**

- customer doesn't get insight how well the hardware is maintained
- what underlying hardware the OS is running on

The customer is responsible for maintaining those OSs and patching software

**Major benefits of IaaS**

- is in terms of **Business Continuity**
- the flexibility of choosing OS installed

## Reflections

### What are the reasons that a company might choose IaaS?

- the company is developing an application on top of an OS that isn't typical or may be unique
- they have to develop the environments themselves

### What is the dividing line for responsibility in IaaS?

Providers are responsible for maintaining the psychical security, hardware and APIs tha customers utilize to access cloud services

Customers are responsible for maintaining the OS that they deploy and any data

### What are advantages and disadvantages of IaaS?

Advantages: fairly low cost of business continuity services, increased flexibility in terms of OS

Disadvantages: lose control of the actual hardware that the service is running from (however someone else is maintaining that, reducing the cost of maintaining the psychical data center, psychical security and utilities)

---

> A threat is anything that can cause damage or disrruption to the cloud based system

> A vulnerability is a weakness that could be exploited by a threat

> A risk is a probability that a threat will exploit a vulnerability

---

## IaaS Specific Risks

### Personnel threats

- Background checks
- Segregation of duties

### External threats

- Malware
- Dos / DDoS
- Man-in-the-middle
- Geographic location

### Lack of specific skill set

- Security over the environments in the cloud
- Operational security practices

**Quiz Question**

What is the most significant risk that a customer can evaluate and control in IaaS?

- Personnel threats
- External threats
- Lack of a cloud specific skill set, Correct

---

## PaaS risks

It's not all easily deployable, development environments and scalable databases

**PaaS risks**

- Interoperability
  - The cloud provider is responsible for updating the OS. Unless there is effective communication between provider and customer, updates can break applications or may not function properly
- Backdoors
  - Since most PaaS are used for development, introducing a backdoor during development is a significant risk. If left unchecked they can go to production environments too.
- Resource sharing
  - Information breach, side channel attacks
- Virtualization
  - introduces various risk when used in PaaS

**Quiz Question**

What security risk may be accidentally introduced during development ?

- Side channel-attacks
- Information bleed
- Backdoors, Correct

Backdoors can be introduced during the testing process and with ineffective management they can potentially left in.

---

## Software as a Service (SaaS)

Components of SaaS

- Applications
- Email
- Customer Relationship Management (CRM)

Customer is only responsible for the data that you put in the app

### Reflection

### What are some SaaS applications that you use every day?

Fitness app that charges monthly or free that sales your data

### What is the dividing line for responsibility in SaaS?

The provider is responsible for maintaining the application. The customer only puts in the data.

### What are the advantages and disadvantages of SaaS?

SaaS applications help businesses focus on what they do best. You give up a lot of the control when you put the data in that SaaS application.

---

## Software as a Service (SaaS) risks

- Proprietary data formats
  - Vendor lock-in
    - ability to switch vendor once you 've started
  - Data portability
    - ability to easily remove information and switch apps
- Web application security
  - Browser
    - Web based browsers exposes many potential threats like stealing user credentials or potentially even injecting code into the platform.
  - API
    - security misconfigurations, data exposure
- Virtualization
  - risks of information bleed, side-channel attacks. Changes on the hardware cache can provide hints to privilege information

**Quiz Question**

- Yearly cost increases
- Proprietary data formats, Correct
- The update schedule

---

## Virtualization threats

Virtualization is the ability to provision and create virtual environments that individual customers and their applications run.

That is done through using on what is called hypervisors

- Hypervisors
  - Type I
    - Runs directly on system hardware, bare metal (e.g. Windows hyper-v, Linux KVM kernel virtual machine)
    - the attacker is limited to the hypervisor and the machine, because all individual machines are beneath the hypervisor, being provisioned by the hypervisor
  - Type II
    - Virtual machines are running on top of a host OS (e.g. VMware, VirtualBox). In this instance, the primary OS has more power than those individual guests OS
    - have a larger attack surface, more vulnerable, attacker can attack the hypervisor itself, the underlying OS and the machine
- Guest escape
  - when a user is about to leave their VM and interact with either the hypervisor or with other VMs.
  - User can potentially edit, view, copy the data of another VM. (PaaS, SaaS a customer can gain access to another customers data)
  - rare because they rely on failure of other controls
- Host escape
  - the user can leave the host machine and access devices on the network
  - that would reflect failure to multiple controls
- Information bleed
  - when an application fails, it may reveal little information about what that application actually is.
  - A user can find out what actually is running on the VM without having access to it

**Quiz Question**
What type of hypervisor would you choose to minimize the attack surface?

- Type III
- Type II
- Type I, correct

---

## Cloud Deployment Models

- Public cloud
  - Any business or individual that wants to purchase hosting services on the public cloud is able to to so.
  - The main benefit is that is cheap, as it utilizes shared resources, it is the most cost effective.
  - But you can lose in terms of control (e.g. multi tenancy, data segregation, maintaining security)
- Private cloud
  - reserved for one organization
  - the hardware may belong to the organization
  - greatest amount of control
  - most expensive
- Hybrid cloud
  - Mix of any of the 3 models used together
  - Linking applications in a ways that enables data sharing
  - an organization may host production in on-premise data center but leverage the cloud for backup solutions
- Community
  - the cloud architecture is shared by several organizations (e.g. research institutions or government)
  - on premise or off premise in terms of it's administration, de-centralized

**Quiz Question**

An organization hosts its production environments on-premise but leverage a dedicated cloud deployment for it's backup and disaster recovery need. What cloud deployment model is this?

- Private cloud
- Public cloud
- Hybrid cloud, Correct

---

## Public Cloud

The benefit is that there is **little cost because it's a multi tenant environment**, meaning multiple customers are running their applications that are running on the same underlying hardware

- Publicly shared

  - Multitenant environment
  - Lower cost, easily available

- Data protection

  - Best for data with lower sensitivity

- Common pubilc clouds
  - AWS, Microsoft Azure, Google Cloud, Oracle Cloud, Salesforce, IBM Cloud, Dropbox, AppleCloud

### What are the reasons that a company might use a Public Cloud deployment model?

They really want an affordable, easily accessible option to do storage or apps that aren't processing highly sensitive information

### What are the reasons a company would want to avoid using a Public Cloud?

It's public! Should encrypt information, cloud platforms and are natively more risky as may be accessed by unauthorized parties

### What are some Public Cloud that you use at work or in your personal life?

Google cloud

## Public Cloud Deployment Risks

- Vendor lock-in

  - That can be addressed by looking an any contract or fine print before using a public cloud, to ensure how easily data can be imported from the public cloud to another vendor

- Vendor lock-out

  - vendors may not have adequate capital to maintain their cloud, and if they go out of business you are locked out, unable to access your data, hardware not connected to the internet

- multi tenant environment
  - Data separation
    - data from multiple customers are saved on the same hardware, misconfigurations or potential vulnerabilities may compromise the potential records
  - Virtualization
    - up to provider to ensure that VMs are protected and hypervisor is well maintained
  - Availability
    - the cloud becomes a target for threat actors with Dos or DDos
  - Encryption
    - encryption keys be compromised

**Quiz Question**

What does multitenancy mean in cloud computing?

- Multiple customers' data can be stored, processed, or archived on the cloud providers hardware, Correct

- Different data types can occupy the same cloud server

- More than one cloud provider can operate out of the same data center

---

## Vendor Lock-in

primary risk factors:

should consider before putting data in the cloud about creating a dependency, effective risk management, business continuity scenarios.

- Lack of portability

- Proprietary data formats

- Physical / technical limitations of moving
  - what if there are petabytes of data, AWS has Snowball

**Quiz Question**

A medical imaging software company is dissatisfied with the service level at its current hosting provider. The company would like to move but the volume of imaging data stored at their current provider would take months to move given the current providers capabilities. This is an example of which vendor lock-in risk?

- Proprietary data format

- Regulatory constrains

- Physical/technical moving limitations, Correct

---

## Vendor Lock-out

primary risk factors:

diligence on venture, their compliance obligations and financial health

- Provide longevity

  - provider is not that mature, or can't maintain their data center and go out of business

- Legislative environment
  - vendors need to meet their compliance, they be fined or shut downed temporarily, vary

## How should your cloud vendor review processes address the risk of vendor lock-out?

## If you were responsible for mitigating the risk of vendor-lock out, how would you do it?

---

## Multitenant Environment Risks

- in a single tenant environment, every single customer has their own instance of the application and their own corresponding database

- in a multi tenant environment multiple customers data is processed **in the same application**. Different customers data can be stored on the same hardware.

primary risk factors:

- Conflict of interest
  - unlike dedicated, the cloud provider is focus on maintaining the environments for all customers, less concern for individuals
- Escalation of privilege
  - when ones customers data is breached, the attacker may escalate their privilege level on the application and recover other piece of data
- Information bleed
  - Failures or malfunctions in an application or database can revile information on application's OS and attackers can use tailored vulnerabilities
- Legal activity
  - when data is on the same server, illegal actions can potentially prevent people from accessing any of the data on that server

**Quiz Question**

An online retailer's website is not working. The IT department discovers that the company can no longer access critical data stored in the cloud. The company soon learns that the data of one of the cloud customers on that hardware was involved in a criminal investigation and the server has been isolated. This is an example of which multitenancy risks?

- Conflict of interest
- Legal activity, Correct
- Information bleed

---

## Private Cloud deployment

most control and protection, higher cost

common characteristics:

- Dedicated hardware and other infrastructure

- Physical data isolation

- Premium price

- Really appropriate for highly sensitive data
  - PII, health data

**Quiz Question**

A company pays a cloud provider to maintain the company's hardware in the cloud provider's data center. What type of cloud model is this?

- Private Cloud, Correct
- Public Cloud
- Platform as a Service (PaaS)

---

## Private Cloud deployment risks

there still are some risks

most relevant risks to private cloud environments

- Personnel threats

  - cloud employees could introduce misconfigurations or security vulnerabilities, malicious code and backdoors
  - cloud provider should do background checks, financial checks on individuals with access to sensitive information

- External threats

  - Dos or DDos, malwares
  - should monitor and have appropriate logging and incident response, as well as patching and configuration of the private cloud

- Regulatory non-compliance

  - particularly important to the private cloud, no multi tenant risks but there might be more obligations to protect that data
  - should have appropriate control mapping, should understand the roles and regulations

- Natural disasters
  - true of any cloud based
  - should have appropriate backup solutions, redundant utilities

**Module reflection**

### How do the risks of a private cloud deployment compare to the public cloud?

Many of these are the same (e.g. Personnel threats, external attacks)

The main difference is the **attack surface**. In public there is greater attack surface because you are relying to virtualization.

### Could private cloud deployments create a false sense of security?

Any organization should be taking security very seriously.
It's important to do diligence on your vendor to prevent some of the internal threats. Make sure that have adequate controls in place to mitigate those risks associated with natural disasters.

---

## Community cloud environments

In the community cloud, one affiliated group of organizations is sharing cloud infrastructure. In most cases, the infrastructure is owned and administered by the affiliated group.

common characteristics:

- Dispersed administration

  - each group it is maintaining it's piece of infra or application and other members of this group get to utilize those resources
  - e.g. research organizations that coordinate and share data or apps

- Security and compliance

  - there can be standardization across the community cloud because the organizations share the same mission, which results in higher level of control and compliance in the cloud

- Shared cost
  - the cost is lower because all the organization are sharing the cost and resources

**Quiz Question**

Which of the follow is the most significant difference between community and public cloud deployments?

- Shared cost
- Shared services
- Organizational affiliation, correct

The common denominator among how community clouds work. There is a shared mission or connection among organizations that participate in the community cloud.

---

## Community Cloud Deployment Risks

Most relevant risks to community cloud environments

- Decentralized administration
  - Improved resiliency but increased attack surface
  - Performance monitoring
    - because it's decentralized, the performance monitoring becomes difficult and can make it difficult to address security incidents
  - Security monitoring
- Access control
  - there isn't a centralized policy to access control
- Configuration management
  - no centralized way of setting the tone of how configuration should be done across the cloud

Improved resiliency: if one node goes down, it doesn't bring the whole cloud down for it's members

**Quiz Question**

Which of the following risks is most central to Community Cloud deployments?

- Free-riding on the shared cost of infrastructure

- Resiliency

- Decentralized administration, correct

---

## Cloud security process

high level steps:

- Identify Requirements

  - this is all about the why, security is all about managing risk and reducing to levels that are acceptable within the organizations risk tolerance
  - how is your business really leveraging the cloud (service, deployment models to expand what they do)
  - what are the inherent risks on what they try to do on the cloud (how will the backups work, how processing activity is going to be monitored, who needs access to this)

- Select Provider, Service, and Deployment Models

  - investigating which vendor meets our needs

- Define Architecture

  - building a picture of all the servers and applications
  - assets that need protection
  - how they communicate to each other and how the communication is protected
  - storage
  - who is managing what

- Assess Security Controls

  - what regulations are applicable to our industry that need to be implemented

- Identify Control Gaps

  - what controls are in place on the on-prem solution and what we need to do in the cloud

- Design and Implement Controls

  - adapt any controls to the cloud to ensure that they meet your organizations business objectives, risk objectives and then any security control requirements based on a framework that you chosen to mitigate risk or legal requirements

- Manage Changes
  - the dynamic aspect of the cloud must me managed as well

**Quiz Question**

- Identify requirements, Correct

- Define architecture

- Designing and implementing controls

---

## Security responsibility by service model

| Responsibility                       | On-Prem | IaaS | PaaS | SaaS |
| ------------------------------------ | ------- | ---- | ---- | ---- |
| Data classification & accountability | Y       | Y    | Y    | Y    |
| Client & end-point protection        | Y       | Y    | Y    | S    |
| Identity & access management         | Y       | Y    | S    | S    |
| Application level controls           | Y       | Y    | S    | N    |
| Network controls                     | Y       | S    | N    | N    |
| Host infrastructure                  | Y       | S    | N    | N    |
| Physical security                    | Y       | N    | N    | N    |

Y: Cloud Customer

N: Cloud Provider

S: Shared between Cloud Customer and Provider

### Common customer's responsibility is data classification & accountability

identifying what is the value of the data, what protections does it require, where is it, how do you ensure that you effectively label data to ensure that data of a certain sensitivity level is protected

### Client & end-point protection

ensuring that all the devices that are going to connect wirelessly to your cloud environment are appropriated monitored for security threats and vulnerabilities. Have antivirus software etc. and are able to connect in a secure manner

### Identity & access management

ensuring that you know everybody that is accessing the cloud environment, who they are, their rights and truly authenticate who they are before granting access to the cloud environment. In addition to setting up technical controls that enforce identify access management, there have to be good governance of policies on the insight of the environment to ensure segregation of duties.
People don't write checks themselves, classic example. Ensure least privilege.

### Application level controls

ensuring that there is a secure development lifecycle, that vulnerabilities in the application are always being tested, patched and monitored

### Network controls

the provider has effective controls to monitor performance and security threats on their network or per segmentation to ensure that customer's data doesn't get commingled (become commonly accessible when they are supposed to remain separated) or customers are able to escalate privilege to get access to other customer's data, a lot of these controls are enforced by the network layer

### Host infrastructure

ensuring that there is proper security over individuals servers and hardware that's running on the host infrastructure

### Physical security

The advantage is that you don't have to worry about the utilities and guns and gates to keep people out of the data centre

There are all the security considerations and how they exist on this gradient of shared responsibility between the cloud customer and cloud provider

**Quiz Question**

Which cloud service model comes with the greatest security responsibility for the customer ?

- SaaS
- PaaS
- IaaS, Correct

---

## Defense in depth

- Management

  - such as policies, how do you categorize data, what are the policies around encryption standards you implement, how is data managed, policies for retention and secure destruction, proper documentation

- Technical

  - actual devices or software or alerts that are implemented on a system to provide control depth

- Physical
  - fencing, lights, full-time security, camera monitoring of the facility

layer controls are really the ideal way to keep your organization safe.

### Control types

- Preventative
  - reduce possibility of a risk going to occur
- Detective
  - detects and identifies violations or incidents that occurring, such as having an intrusion detection system
- Corrective
  - any control that's really used to remediate or fix a risk, such as failover to another location
- Deterrent
  - discourages violations, lights or signs
- Recovery
  - system recovery or information
- Compensating
  - e.g. another means of capturing meta information

**Quiz Question**

The cloud provider has the greatest control and responsibility over which control type?

- Management
- Technical
- Physical, Correct

---

## Cloud security frameworks and standards

- ISO 27000 (27017 Cloud standards)
  - they reflect the EU regulations, required in some countries, costly but international
- fedRAMP
  - US standards, US governments need it to participate in the cloud services, very expensive
- Cloud Security Alliance (STAR)
  - Security Trust Assurance at Risk, freely available, when you undergone a third party assessment you can publicly register it

**Quiz Question**

Which framework would be best for a multinational corporation operating cloud environment in different geographic regions

- ISO 27000 (27017 Cloud standards), Correct
- Cloud Security Alliance (STAR)
- FedRAMP

---

## Cost benefit analysis

benefits of cloud computing

- Personnel costs
  - on-prem you will need people to maintain the hardware, configure the networks, monitor, make sure applications are secure, utilities are properly setup, effective redundancy
  - the cloud provider takes on many of those costs associated with employees
- Operational costs
  - cost that come with maintaining the hardware
- Regulatory cost Transfer
  - the cost that comes with making sure you have certain controls in place are transferred to the cloud provider
- Capital Expenditure
  - you don't need to purchase all this hardware

---

## Developing business requirements

- Functional requirements

  - Devices
    - might be identified by working with cloud architect to figure out the diagram of the application
  - Processes
    - working with stakeholders to identify what is the business trying to achieve, how the processes that make that happen currently work, what are the inputs and outputs or product
  - Employees
    - what are the employees roles and responsibilities in the overall project, do we have the employees we need

- Nonfuctional requirements

  - expected behavior
    - base line levels of logging, monitoring, performance

- Security requirements
  - we should be thinking of security as an aspect of product quality that should be included as early as possible

You have to keep in mind: what is the business trying to achieve and what is the level of security really appropriate given the value and the business case

**Module reflection**

- How are business requirements determined in your organization?

- How does understanding business requirements improve security?

---

## Business impact analysis

a cornerstone process for establishing effective security in the cloud

to justify going to the cloud is doing cost benefit analysis and ensure that benefits really make sense

business impact analysis ensures that security is well set up to properly defend the assets that are being deployed in the cloud

**Business Impact Analysis Process**

- Establish existing state

  - asset inventory
    - gather all network diagrams or artifacts that describe the processes that are involved in the existing state of the organization, applications, databases, servers, load balancers
  - interviews
    - interview people that maintain critical parts in the existing state, collect network traffic
  - regulations
    - laws you have to adhere

- Determine criticality

  - what assets are most essential, the crown jewels of the organization which are the elements which deserves the most protection

- Establish risk appetite
  - avoid
    - we are not going to pursue that
  - accept
  - transfer
    - companies now have cyber security breach insurance
  - mitigate
    - controls decrease the likelihood of the risk or the potential impact of the risk to an acceptable threshold

**Module reflection**

- Does your organization have an asset inventory?

- What is the most critical asset in your organization ?

- How are risks identified, evaluated, and monitored ?

---

## Developing security requirements

### Business requirements

business requirements will help you determine how the CIA framework will be enforced and maintained

### Business impact analysis

then we leverage the business impact analysis to identify what are the most critical assets and how to prioritize security efforts and requirements

### Frameworks

Many organizations have figured out the high level control areas that really deserve our focus such as encryption, access, data classification, labeling, redundancy, backups. These areas are a little different compared to On-Prem

### Regulations

What unique controls apply to you and the business case

**Module reflection**

- How does your organization identify security requirements?

- How could the different security responsibilities we have discussed be used to proactively identify security requirements?

Different shared responsibilities can help us create a shortcut for identifying the most important security requirements for the organization

---

## Domain 1 Summary

**Module reflection**

- What is the cloud computing and its benefits?

- What are the three service models?

- What are the four deployment models?

- What is the shared responsibility model and why is it important?

- How do you demonstrate the business value of the cloud?

- How do you identify and meet your organization's security responsibilities in the cloud?

---
