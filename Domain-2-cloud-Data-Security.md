# Domain 2: Cloud data security

**Domain 2 topics**

- Data classification
- Data lifecycle
  - stored, processed, created, shared etc.
- Cloud data storage
- Cloud data security strategies

**Quiz Question**

What is the first step to effectively protect cloud data?

- Classification, Correct
- Creation
- Encrypt

---

## Data classification

- Criticality
- Category
  - Functional
  - Regulated
- Jurisdiction
  - the cloud services are in different geographic regions, that means that data are in different legal jurisdictions when it comes to security and legal process securing and maintaining as evidence
- Public Sector
  - Top Secret
  - Secret
  - Classified
  - Unclassified
- Private Sector
  - Confidential
  - Private
  - Sensitive
  - Public

Without effective data mapping you can't effectively manage data security.

**Quiz Question**

What is the highest data sensitivity level in the private sector data classification scheme?

- Top secret
- Confidential, Private sector
- Proprietary

---

## Data roles

- Data Owner
  - they own all aspects from protecting that data
- Data Custodian
  - the person applying and maintaining any of the technical controls and labeling (network administrator, security team)
- Data Processor
  - an organization or individual application that manipulates, stores or moves data on behalf of the data owner (from legal perceptive, the cloud provider), if it's in your system you are the data processor
- Data Subject
  - the individual to whom the data relate or respond (e.g. when you put information to a SaaS, you are the data subject)

Data Custodian executes the will of the Data Owner when it comes to enforcing security requirements as well as changes to data classification.

Data Processor is the organization that is manipulating or storing the data of individual Data Subjects

Data Subjects are granted certain rights and protections depending on the jurisdiction

**Quiz Question**

A system administrator wants to change the classification of a data table because new business priorities have made the information less relevant. Who should the administrator contact before relabelling and moving the data?

- The administrator has the latitude to move data and label data as business needs change.

- The data owners ultimately decides the appropriate data label and storage location

- The data owner should decide the label but the data custodian should implement the appropriate protections and storage, Correct

---

## Cloud Data Lifecycle

- Create
  - ensure data is classified
- Store
  - Data At Rest, needs to be encrypted to ensure that is properly protected
- Use
  - Data In Use
- Share
  - Outside the organization, or inside the cloud between application
- Archive
  - Having an effective retention policy
- Destroy
  - Should be destroyed securely

When data is created, if it's outside the cloud and needs to be transmitted to the cloud. Data is in the state of Data In Transit.

**Quiz Question**

- Create, use, store, share, archive, destroy

- Create, store, share, use, archive, destroy

- Create, store, use, share, archive, destroy, Correct

---

## Data discovery

- Label-based

- Metadata-based

- Content-based
  - data labeling software

**Module reflection**

- How does your organization identify and label data?

- How can we leverage the increasing importance of data analytics to improve data security?

---

## Cloud data security strategies

- Encryption

  - ensure confidentiality and integrity of data

- Masking

  - render data in a state that people can't infer completely what the sensitive information is

- Security information and event management (SIEM)

  - monitor events that are happening regarding data in the Cloud Based environment.

- Egress monitoring
  - while exiting or leaving, data loss prevention, digital rights management

**Quiz Question**

Obscuring the digits of a credit card number is an example of which data security strategy?

- Encryption

- Egress monitoring

- Masking, Correct

---

## Encrypting Data

The cryptographic process of rendering text information unreadable and the only way to render back to clear text is with a use of a decryption key.

**Encryption stages and methods**

- Encryption at rest

  - Whole-instance encryption
    - the entire piece of hardware is encrypted, workstations such as laptops, if it's stolen the thief won't be able to retrieve information
  - Volume encryption
    - encrypting a particular volume of data, e.g. certain set of files, ensures confidentiality

- Encryption in transit

  - Transport Layer Secure (TLS)
  - Secure Sockets Layer (SSL deprecated in 2015)

- Encryption in process

  - holomorphic
    - data which is encrypted but can actually be processed

- Advanced Encryption Standard 256
  - current standard, secure and appropriate

**Quiz Question**

Which term refers to the process of performing calculation on data while still encrypted

- Homomorphic, Correct

- Hologramic

- Metacryptic

---

## Encryption types

**Types of encryption**

- Symmetric

  - only one key which is used to encrypt the data and decrypt
  - very fast but how you ensure that the other party has the key, also how do you know the sender is who they say they are

- Asymmetric
  - pair of public-private key, slower but more secure
  - the other party has only the public key
  - asymmetric encryption is used to send a symmetric key

**Quiz Question**

A company has a private cloud instance. If a third-party wanted to send them an encrypted message they would need to use which key?

- The company's public key, Correct

- The third-party's private key

- The third-party's public key

Companies use their public keys enabling other organizations to encrypt information that they can safely decrypt using their private keys

---

## Encryption and key management

**Key management**

- key escrow
  - typically a third vendor party is used to maintain the encryption keys for an organization or keys can be maintained in a non cloud environment location
- key recovery
- key distribution
- key revocation
  - if a key becomes compromised, you need to register that breach with the CA
- outsourced key management
  - cloud access security brokers help with the authentication and key management

encryption in transit should be used for encryption keys to be communicated

**Quiz Question**

Where should you never store your encryption keys?

- On-premise

- With a CASB

- In the cloud with data it encrypts, Correct

The keys should be always kept separate from the data that protects

---

## Federal Information Processing Standard (FIPS PUB 140-2)

FIBS PUB 140-2 standard is set by the US government for approving cryptographic modules.

A system that is **compliant** may meet the 1 to 4 level scheme

A system that is **validated** it's actually tested.

- Level 1
  - No specific physical security
- Level 2
  - Show evidence of tampering, meaning someone attempted to manipulate or mess with the integrity of the device
- Level 3
  - Prevents the intruder from gaining access to CSPs (Critical Security Parameter)
- Level 4
  - Complete envelope of physical protection
  - Detects and responding unauthorized physical access attempts
  - Detect penetration and deletes plaintext CSP

**Quiz Question**

Which FIPS 140-2 level prevents intruders from accessing the CSP but does not delete the CSP upon detecting a penetration?

- Level 2
- Level 3, Correct
- Level 4

---

## Hardening devices

decreasing the attack surface, key strategies for protecting data

**Hardening techniques**

- Guest accounts removed
- Unused port should be closed
- No default passwords
- Strong password policies
- Secure admin accounts with logging
- Control physical access
- Appropriate patching
  - many businesses are hesitant with patching, it can break systems, disrupt the performance of applications that customers are using
  - double edged sword but organization should try to patch major critical vulnerabilities as soon as possible

**Module reflection**

- How are hardening standards enforced at my organization?

- How certain am I that hardening standards are consistently applied?

  - Amazon has AMI

- How are hardening standards monitored at my organization?
  - port scanning

---

## Jurisdiction requirements

Data centers are all over the world, in different zones. The benefit that comes with having a geographically dispersed set of cloud resources is that you can have redundancy and backup, but one of the pitfalls is that different jurisdictions have different requirements.

**Geographic jurisdictions**

- Different rules about transparency

  - EU has rules about ISP services, ISP can't privilege the access of one of the customers over another or if there are some differences in term of speed between customers the ISP has to publish a justification

- Conflicting standards

- Managing jurisdictional complexity
  - In a multinational firm, your legal and compliance department needs to be in sync with regarding how the cloud data is stored or set up to utilize different geographic areas

**Module reflection**

### How might understanding jurisdictional requirement help to address strategic risk?

### Is your legal/compliance department aware of your cloud legal risks?

---

## Protecting data in transit

**Secure data in transit**

- Encryption in transit

  - Transport Layer Secure (TLS)

- Link/Network Encryption

  - each different node along the network they are hitting information is encrypted
  - VPN

- Client/Application Encryption

  - Encryption applied before transit

- Proxy-Based Encryption
  - Data is transmitted to a proxy application or server which encrypts before sending further on the network

**Quiz Question**

Which of the following creates an encrypted tunnel for secure data transit?

- Virtual private network, Correct

- Application encryption

- Proxy-based encryption

---

## Data storage architecture

**Common methods include:**

Volume and object storage are mainly found in IaaS.

In volume storage you typically encrypt and store large volume of information that's attached to a particular instance, an instance being a virtual hard drive or a piece of infrastructure.

Some volume storage are so large that multiple containers (partitions) are used to cover the information.

This has a benefit when it comes to security which is called **data dispartion**, which supports resiliency and security because when data is stored in the cloud in multiple instances they are usually backed up and in case one region goes down will be able to recover quickly.

- Volume storage

  - File storage
  - Block storage

- Object-based storage

  - Objects
    - makes data labeling very easy
  - Metadata

- Databases

  - In PaaS and Saas databases are typically used to access information

- Content delivery network (CDN)
  - Caching
  - High performance

---

## Data retention policy

Organizations retention strategy is the governance level control that will drive how data is retained in a way that reduces operational costs, ensures that data is properly protected and that the company doesn't assume too much risk by keeping data longer that it should.

Data retention policy should lay out:

- Retention period
  - data used for protective purposes can go stale quickly, data 2 years old might be not that relevant
- Applicable regulation
- Retention formats
  - when data go into archive state, what should the format be and where is stored into the cloud architecture
- Data classification
  - how should the data be stored, different locations or ways
- Archiving and retrieval procedures
  - define policies for retrieval for legal reasons
- Data deletion procedures and mechanisms
  - Protects from legal risk
- Monitoring, maintenance, and enforcement

**Module reflection**

- When was the last time you read your organization's data retention policy?

- How can an effective data retention policy enhance security, analtics, and risk management?

---

## Data Destruction Methods

How do we ensure that data is truly gone:

- Physical destruction
  - the most secure way of destorying data
- Degaussing
  - powerful magnets which renders the information unreadable on the disk
- Overwriting
  - example of data deletion, not necessarily data destruction when applied
- Crypto-shredding (cryptographic erasure)
  - is the main standard for properly destroying data in the cloud, is deleting all the keys that are used to decrypt the data

**Quiz Question**

Which of these deletion methods is used in public cloud deployments?

- Physical destruction

- Ovewriting

- Crypto-shredding, Correct

---

## Audibility, traceability, accountability

Auditing is the ability to look through processes, activity access controls but basically is tight individual actions to changes

Auditing ensures that controls that are in place are working effectively

- Auditing
  - Non repudiation, to show individuals took particular actions or the same for threat actions
- Database activity monitoring (DAM)
- File activity monitoring (FAM)
- Accountability
  - detect when policy violations occur
- Prevents waste

**Module reflection**

- What is your relationship like with the auditing/compliance function at your organization?

- Is auditing being used effectively to improve operations, security and policy enforcement?

---

## Data Audit Policy

**Audit policy**

Auditing is about being able to enforce traceability and non repudiation when it comes to actions taken within environments.

- Audit periods
  - the amount of time the audit will go through
- Audit scope
  - what is being audited, usually entails hardware, data, people etc.
- Audit responsibilities
  - internal
  - external
    - easier to maintain independence with external auditors so they are less objective about the evaluation and quality of evidence
  - regulations
  - chain of custody
- Audit processes & procedures
  - visibility and quality risks in the cloud, more difficult in the cloud based environments
- Monitoring, maintenance, and enforcement

**Quiz Question**

A SaaS company has started to use a new cloud service provider for storage. What is the primary aspect of the audit that this would this affect?

- Audit period
- Audit responsibilities
- Audit scope, Correct

---

## Data Privacy

**Use cases and reasons for data privacy controls**

- Personally identifiable information (PII)
  - Sensitive PII
- Data collection
  - Purpose
  - Use limitations
  - Openness
- Accountability
  - organizations must be accountable for anything that may disrupt the privacy of individual customers or employees, notification rules with strict criteria

PII includes: Name, email, home address, phone

Sensitive PII includes:

If Stand-Alone

- Social Security Number
- Driver's license or stat ID #
- Passport number
- Alien Registration Number
- Financial account number
- Biometric identifiers

If Paired With Another Identifier:

- Citizenship or immigration status
- Medical information
- Ethnic or religious affiliation
- Sexual orientation
- Account passwords
- Last 4 digits of SSN
- Date of birth
- Criminal history
- Mother's maiden name

---

**Quiz Question**

Which of the following is not PII?

- Mother's maiden name, Correct
- Home address
- email address

---

## Privacy Safeguards

**Data privacy considerations and safeguards**

- Minimize personally identifiable information (PII)
  - Collection
  - Use
  - Retention
- Privacy impact assessment
- Safeguards
  - De-identification
    - changing records in a way that PII is removed
  - Generalization
    - making data less precise, can be implemented in a role base level
  - Suppression
    - deleting entire records so PII is gone
  - Noise
    - add random data to strings of information that could contain PII
  - Swapping
    - exchanging certain data or one field of a record with another field
  - Replacement
    - replacing data with average values or remove data when not necessary

**Module reflection**

- What PII does your organization collect?

- What privacy safeguards does your organization use, or should be using, to protect privacy?

---
