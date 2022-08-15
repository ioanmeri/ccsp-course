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

## Open-source software

what to use depends on the context, cost benefit analysis, more secure or flexibility

- Proprietary vs open-source
  - open source if freely available, it can be modified, reviewed
  - in proprietary you pay premium fee to get access
- Vulnerabilities
  - in open source software, threat actors can design their own exploits
  - in proprietary, difficult to have attribution for vulnerabilities
- Flexibility
  - in open source should do testing and validation to ensure there are no known vulnerabilities

**Quiz Question**

Which of the following is not a benefit of open-source software?

- The ability to customize security
- Vulnerability discovery
- Vulnerability attribution, Correct

---

## Sandboxing

in can be the physical isolation to do development or testing

or can refer to logical isolation, processes isolation

**Sandboxing in the cloud context**

- Testing
  - prevents tests from affecting other systems, analysis or forensics
- Environment separation
  - keep testing and development separate from production to not introduce vulnerabilities
- Code isolation

**Module reflection**

- What examples of sandboxing have you observed?

- Are there instances that you now see could benefit from sandboxing?

---

## Cloud application security testing concepts and methods

**Security testing methods and tools**

methods include:

- API approval and management
- Secure open-source
- Threat modeling
  - what are the potential vulnerabilities
- Software security testing
  - active and passive methods
- Quality of Service (QoS)

**Which of these concepts represents the trade off between application security and productivity?**

- QoS, Correct
- Software security testing
- STRIDE

You don't want applications so secure that it downgrades the overall quality and performance of the software

---

## OWASP top 10

Open Web Application Security Project, enables organizations to maintain the standards for application security

- Injection
- Broken authentication
- Sensitive data exposure
- XML external entities (XXE)
- Broken access control
- Security misconfiguration
- Cross-site scripting (XSS)
- Insecure deserialization
- Using components with known vulnerabilities
- Insufficient logging & monitoring

**Quiz Question**

Which of the follow is not in the OWASP top 10?

- Injection
- Broken authentication
- Denial of service, Correct

---

## OWASP top 10 (1): code injection

**Code injection**

malicious code is entered into a field

- Handling of untrusted data
  - Character
  - Data
  - Amount of data
  - Legacy code
- Impact
  - Loss of confidentiality
  - Loss of integrity
  - Loss of availability
  - Loss of accountability

measures to tackle this problem: input validation, effective code review, security testing

**Quiz Question**

The risk of code injection can be mitigated through which of the following?

- Input validation, Correct
- Process isolation
- Special character requirements

can corrupt data and the system, unauthorized access, covering tracks

---

## OWASP top 10(2): broken authentication

**Broken authentication**

- Credential configuration
  - Dictionary attacks
  - Bruteforce attacks
  - Default accounts
  - Unexpired session tokens
- Prevention
  - MFA
  - Do not use default password
  - Weak password checks
  - Loss of accountability
  - Limit failed logins

**Quiz Question**

When an attacker has a potentially valid list of usernames and passwords to use against a system?

- Valid list attack
- Credential stuffing, Correct
- Rainbow table

rotate usernames and password, not use the same usernames passwords, use long strong passwords

---

## OWASP top 10(3): Sensitive data exposure

**Sensitive data exposure**

- Sensitive data
  - Transit risks (HTTP, SMTP, FTP)
  - Weak cryptographic algorithms
  - Lack of certificate validation
- Prevention
  - Classification
    - what data is sensitive
  - Get rid of unnecessary sensitive data
  - Encryption at rest
  - Encryption in transit
  - Verify configuration effectiveness

**Quiz Question**

What is the most important control for preventing sensitive data exposure in web applications?

- Encryption in transit
- Server side certificate validation
- Classification, Correct

---

## OWASP top 10(4): XML external entities (XXE)

**XML external entities(XXE)**

- Extensible markup language(XML)
  - Extract data
  - Execute commands
- Prevention
  - Training
  - Patching
  - XSD validation
  - API security gateway

**Quiz Question**

An XXE attack can be used to do all of the following except?

- Denial of service
- Data extraction
- Impersonation, Correct

---

## OWASP top 10(5): Broken access control

**Broken access control**

- Access control bypass
  - URL modification
  - Primary key substitution
  - Meta data manipulation
  - APIs with missing access controls
- Prevention
  - Prevent modification of the access control check or meta data

**Quiz Question**

Broken access control exploits can be used to do all of the following except?

- Denial of service, Correct
- Escalation of privilege
- Impersonation

---

## OWASP top 10(6): Security misconfiguration

leads to unauthorized access and reconnaissance

- Configurations
  - Lack of hardening
  - Improper permissions
- Prevention
  - Hardening
  - Patching
  - Training

**Quiz Question**

Addressing security misconfigurations by removing default accounts, passwords, and services is also reduces which of the following?

- Hypervisor
- Cloud costs
- Attack surface, Correct

---

## OWASP top 10(7): Cross-site scripting

a malicious actor takes advantage of a trust of a user has in a website

- Steal
  - Credentials
  - Session token
  - Cookie
- Prevention
  - Frameworks that automatically escape XSS
  - Escape untrusted HTTP request data
  - Context-sensitive encoding

**Quiz Question**

Which type of XSS attack allows the attacker to execute arbitrary HTML in the victim's browser

- Reflected, Correct
- Stored
- DOM

---

## OWASP top 10(8): Insecure deserialization

Serialization is the process of translating a data structure or object into a state that can be stored and transmitted and reconstructed later(deserialization)

An attacker inputs a malicious code or string in the serialized object that is activated upon deserialization

Can result to remote code execution

- object and data structure manipulation
- Prevention
  - Not to accept serialized objects for untrusted sources
  - Restrict and monitor servers that deserialize

**Quiz Question**

Which of the following is potentially vulnerable to deserialization exploits?

- Applications
- APIs
- All of the above, Correct

---

## OWASP top 10(9): Using components with known vulnerabilities

- Vulnerabilities
  - Versions and dependencies
  - Unsupported software
  - Lack of scanning and patching
- Prevention
  - Patch
  - Remove anything unnecessary
  - Keep a software inventory
  - Monitor libraries

**Quiz Question**

What does CVE stand for?

- Common vulnerable execution

- Common vulnerabilities and exposures, Correct

- Change vulnerable exposure

Year discovered, number, identifier

---

## OWASP top 10(10): Insufficient logging and monitoring

- Logging
  - Logins and failures
  - No warnings or review
  - No log storage
- Prevention
  - Capture the right logs
  - Configure alerts
  - Establish incident response

When having a penetration test, make sure that the security team is able to piece together and identify the steps of the penetration tester took by examining the logs

**Quiz Question**

How long did it take on average to identify a breach in 2016?

- 150 days
- 191 days, Correct
- 239 days

---
