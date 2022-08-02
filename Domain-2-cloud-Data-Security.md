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
