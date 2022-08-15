## Cloud application security

**Domain 4 topics**

- Application security threats
- Secure software development
- Identity and access management
- Cloud application technologies
- Application security testing

**Module reflection**

- What cloud applications are you responsible for protecting?
- What are the steps of your software development life cycle?
- How are application security threats identified at your organization?

---

## Challenges of cloud application deployment

- Performance issues
  - in the cloud bandwidth is a limiting factor, for on-prem code might not be designed as efficiently
- Cloud ready?
  - code need to be fixed and optimized for cloud, encryption may need to be employed in the cloud for data in transit, at rest and in process
- Documentation
  - not adequate docs for deploying
- Secure APIs
- Tenancy separation
  - emphasis on isolation techniques, access control, secure remote administration to avoid data bleed

**Quiz Question**

Which of the following refers to moving an application to the cloud without changing any of the underlying code?

- Forklift, Correct
- Cloud transplant
- Cloud shift

---

## Training and awareness

- Training vs. awareness
  - awareness is building a familiarity with what constitutes insecure configurations, best practices // training is more specific, how to implement the concepts
- Hosting in the cloud
- Cloud specific training
  - asses people skills, code reviews

**Module reflection**

- Which cloud applications does your organization maintain?
- What training do developers at your organization receive regarding secure cloud development?

---

## Cloud software development life cycle (SDLC)

- Analyze
- Design
- Develop
- Test
- Deploy
- Maintain

**Quiz Question**

Change management in this stage of the SDLC is essential for security and performance?

- Design
- Deploy, Correct
- Maintain

---

## Secure software development life cycle (SSDLC)

security is part of product quality

- Define
  - security application architects
- Design
  - secure manner of user stories
- Development
- Testing
  - look for vulnerability, functional testing
- Secure operations
  - administrative aspects, e.g. configuration changes need to go through a process, deployment environment is monitored
- Disposal
  - end of life of software, how to deprecate

**Quiz Question**

What is the most important step in the SSDLC from a security perspective?

- Design
- Secure operations
- Define, Correct

---

## Application security standards (ISO/IEC 27034-1)

**ISO 27034-1 standard**

- International organization for standardization (ISO)
  - it has two documents the ONF and ANF
- Organizational normative framework (ONF)
  - security controls, best practices, principles for development activities
- Application normative framework (ANF)
  - specific version of ONF for a given application

**Quiz Question**

ONF-to-ANF relationship is which of the following?

- one-to-one
- two-to-one
- one-to-many, Correct

The organization needs a global Organizational Normative Framework and each application needs it's own Application Normative Framework

---

## Identity and Access Management (IAM)

two different tasks

- Identify management
  - Identify
  - Identity repository
- Access management
  - authenticate
  - authorize
    - mechanism that enforces the least privilege
  - policy management
    - sets the roles and responsibilities, appropriate access
  - federation
    - trust between organizations

**Quiz Question**

Which of the following is the correct order to steps to evaluate a users access to a cloud-based system?

- Authenticate, identify, authorize
- Identify, authenticate, authorize, Correct
- Authorize, authenticate, identify

---

## Multifactor authentication (MFA)

a security best practice, which is used to strengthen the authentication step of IAM, extra layer of security

for critical systems and administrations, banking, financial

**The four authentication factors**

- Something you know
  - e.g. password
- Something you have
  - authentication tokens
- Something you are
  - biometric authentication
- Something you do
  - you are not a robot

**Quiz Question**

Which of these items is an example of multifactor authentication?

- An iris scan and palm scan
- Username and password
- A password and authentication code, Correct

---

## Single sign-on and federated identity management

Problem is that continually having to going through the IAM process to different applications or servers (although very secure) it declines the operation efficiency.

both techniques are used to provide authorization across devices or group of organizations

**Federated identity management vs single sing-on (SSO)**

**Single sign-on**

is used to typically through one authentication server or service to authenticate the user across all the apps or websites

- saves a lot of time
- increases the security risk, stricter IAM processes needed (MFA)

**Federated identity management**

is taking the single sign-on notion of identity management and pushing it out between multiple organizations

- Identity Provider (IdP)
  - organization itself acts as the IdP, authenticating user
- Service Provider (SP)
  - trust between IdP and SP is what enables multiple organizations to share user access rights amongst them. Due diligence to third party vending is needed that they have adequate monitoring.
  - getting access to multiple organizations, extends the scope

**Quiz Question**

Trust between which parties makes federated identity management possible?

- Between identity providers
- Between service providers
- Between the identity provider and the service provider, Correct

---

## Federation standards

mutual authentication between organizations

- Security assertion markup language (SAML)
  - based on XML
  - allows verification, validation, authorization between organizations
  - if user already signed on organization A, doesn't have to create a unique identity in organization B, SAML creates that level of trust
- WS-Federation
- OAuth
  - for mobile
  - to grant third party tools limited access to services such as http
- OpenID Connect
  - often used for applications and inner website communication

**Quiz Question**

Which of the following federation standards is XML based?

- OAuth
- SAML, Correct
- OpenID Connect

---

## Application programming interfaces (APIs)

depends on the needs of the application

**API types**

- Representational state transfer - RESTful
  - scaling connections between web apps and users
  - 70% are REST
  - flexible, not relying on a single programming language
  - is point to point (end point to db or app over http)
  - stateless
  - best for low bandwidth scenarios
- Simple Object Access Protocol (SOAP)
  - designed to exchange well structured information
  - can work on http, smtp, ftp
  - slower
  - support stateful operations
  - async, not one to one

secure properly to avoid data leakage

**Quiz Question**

Which API type is reliant on XML?

- SOAP, Correct
- RESTful
- JavaScript

---

## API approval and management

**Approving and managing APIs**

- Risks
  - data leakage
  - poor authentication
  - application failure
- API testing
- Supply chain API risks
  - API gateway

audit third party APIs, set the standards for testing the security

**Quiz Question**

Which organization certifies the security of APIs?

- NIST
- ISO
- There isn't one, Correct

---
