# Cloud security operations

- Change management
- Monitoring security operations
- Incident response
- Major cloud risks

**Module reflection**

- What are the roles and responsibilities of cloud security operations?

- What are the aspects of cloud security operations?

- What aspects of cloud security operations surprised you?

---

## Change and configuration management

**Configuration management**

is the approach of setting secure baselines (version, defined images, security requirements etc) for systems and software in the cloud

**Change management**

is the process of making updates or changes, must be reviewed, approved and tested

- Configuration management
  - Baselines
- Change management
- Exceptions
  - in configuration management there may be incidents where users, projects or functions need to use a system or version of software that deviates from the configuration baselines best practices
  - document exceptions and deviations
  - monitor deviations
  - sandbox processes

**Module reflection**

- How is configuration management done at your organization?

  - The difficult part is discipline within organizations to define configuration and hardering standards and monitor deviations

- What is the process for handling configuration deviations?

---

## Change management

- Governance
  - Change management board (CMB)
  - Change control board (CCB)
- Process
  - Baseline
  - Change request
    - a ticketing system, evaluate impact and discuss
  - Change board meeting
  - Change testing
  - Change deployment
  - Change confirmation and documentation
    - so can roll back
- Monitor for deviations

Should be a segregation of duties from those who request a change and those who implement the change when authorized

**Module reflection**

- What is your change management process?

- How do you monitor for unauthorized changes?

---

## Security operations center (SOC)

- Monitoring network security and performance
- Physical access
- Monitoring and log analysis
- Continuous monitoring

SIEM usually located in SOC, firewall logs, strange deviations of the network baseline, IDS & IPS

**Quiz Question**

Which of the following is a best practice for an effective security operations center?

- Continual monitoring and testing of control effectiveness, Correct
- Management review of logical access checks to ensure thoroughness
- Simulated incident response sessions

---

## Incident response

The goal of the incident response process is to minimize the loss of valuable assets, data / availability / damage to business operations. Also to restore availability and prevent any further damage.

- Preparation
- Identification
  - declare an incident
- Containment
  - start clean-up
  - easier in the cloud to isolate and spin down a particular service / server
- Eradication
  - finish clean-up
  - should preserve important evidence
  - ensure non repudiation
  - utilize third party that specializes in digital forensics
- Recovery
  - back in production
- Lessons learned

**Module reflection**

- Have you read your incident response process?

- Who is responsible for declaring an incident?

---

## Treacherous 12

- Data Breaches
- Data Loss
- Account of Service Traffic Hijacking
- Insecure Interfaces
- Denial of Service
- Malicious Insiders
- Shared Technology Vulnerabilities
- Insufficient Due Diligence
- Insufficient Identity, Credential & Access management
- System vulnerabilities
- Advanced Persistent Threats
- Abuse & Nefarious Use of Cloud Services

**Quiz Question**

Which of the treacherous 12 is most easily addressed?

- Advanced persistent threats
- Insufficient due diligence, Correct
- Denial of service

---

## Treacherous 12(1): Data Breach

Disclosure, access or having confidential information stolen

- Impacts
  - Forensics costs
  - Lawsuits
  - Reputational damage
- Controls
  - Policy
  - Training
  - Secure configuration
  - Monitoring
  - Incident response

**Quiz Question**

What is the global average costs of a data breach?

- 10.7 million
- 3.8 million, Correct
- 900 thousand

---

## Treacherous 12(2): Insufficient Identity, Credential and Access Management

- Impacts
  - Compromises all aspects of STRIDE
  - Disrupt operations
  - Modify or delete data
- Controls
  - Encryption and key management
  - Training
  - Password management and MFA

**Quiz Question**

Which of the following is the most effective control against IAM vulnerabilities?

- Multifactor authentication, Correct
- Biometric authentication
- Federated authentication

---

## Treacherous 12(3): Insecure APIs

- Impacts
  - Availability
  - Confidentiality
  - Integrity
- Controls
  - Testing
  - List of trusted APIs
  - Third-party API awareness

**Quiz Question**

How many records were exposed in the 2015 IRS breach because of a vulnerable API?

- 4 million
- 900 thousand
- 300 thousand, Correct

---

## Treacherous 12(4): System Vulnerabilities

- Impact
  - Common vulnerability scoring system
  - Low 0.1-3.9
  - Medium 4.0-6.9
  - High 7.0-8.9
  - Critical 9.0-10.0
- Controls
  - System inventory
  - Patch management
  - Active security assessments

**Quiz Question**

Which is the correct range for high impact vulnerabilities based on the common vulnerability scoring system(CVSS)?

- 9.0-10.0
- 7-8.9, Correct
- 4.0-6.9

---

## Treacherous 12(5): Account hijacking

- Impacts
  - Eavesdrop
    - on transactions, transmissions
  - Steal data
  - Launch new attacks
- Controls
  - Training
  - MFA
  - Account management
  - Application security testing

**Quiz Question**

Which of the following is the most common type of account hijacking attack?

- Cross-site scripting (XSS)
- Cross site request forgery(CSRF)
- Phishing, Correct

---

## Treacherous 12(6): Malicious insider

- Impacts
  - Future compromises
  - Increase costs
  - Waste resources
- Controls
  - Training
  - Segregation of duties
  - Least privilege
  - Logging and monitoring

**Quiz Question**

Limiting certain users' access to a cloud database to read only because they need to review transactions is an example of what principle?

- Least privilege, Correct
- Segregation duties
- Mandatory vacations

---

## Treacherous 12(7): Advanced Persistent Threats (APTs)

Nation state affiliated groups to act to execute a mission to compromise the computer network infrastructure of foreign government or companies

The fifth domain of warfare

- Impacts
  - Intellectual property
  - Espionage
  - Tactical advance
- Controls
  - Threat intelligence
  - Training
  - Knowing the attack surface

**Quiz Question**

The Russian ATP group believed to have compromised the US Federal government systems in 2020, including the Treasury was called what?

- Fozy bear
- Fancy bear
- Cozy Bear, Correct

---

## Treacherous 12(8): Data Loss

- Impacts
  - Lawsuits
  - Reputational damage
  - Business failure
- Controls
  - Business continuity
  - Disaster recovery

**Module reflection**

- What is your data backup schedule?

- Do you have an effective backup strategy?

---

## Treacherous 12(9): Insufficient Due Diligence

The process of evaluating inherent risks or shortcomings associated with vendors, partners, technologies etc.

Locations and data centers can result to regulatory penalties

- Impacts
  - High costs
  - Lack of performance
  - Compliance failures
- Controls
  - Define the process
  - Create a check list

**Module reflection**

- What is your due diligence process?
- What mechanisms are in place to enforce appropriate due diligence?

---

## Treacherous 12(10): Abuse of Cloud Services

When lose control partially or threat actors are able to create and attribute fraudulent transactions to pay for unused cloud services

- Impacts
  - Availability
  - DDoS
  - Phishing campaigns
- Controls
  - Logging and monitoring
  - Incident response
  - Fraud detection

**Quiz Question**

Abuse of cloud services is least likely to result in which of the following?

- Denial of service
- Phishing attacks
- Data deletion, Correct

---

## Treacherous 12(11): Denial of Service

- Impacts
  - Availability
  - Damage to reputation
  - Economic and human capital costs
- Controls
  - Monitoring
  - Baselines
  - Application security

**Quiz Question**

How many terabit-per-second (Tbps) was the largest DDoS attack ever recorded?

- 1.35 Tbps
- 2.3 Tbps, Correct
- 4.3 Tbps

---

## Treacherous 12(12): Shared Technology Vulnerabilities

- Impacts
  - Multitenancy
  - OS
  - Vendors
- Controls
  - Patching
  - IDS/IPS
  - SIEM

**Module reflection**

- How many third-parties are you leveraging in the cloud?

---

## Summary

- Change management
- Monitoring security operations
- Incident response
- Major cloud risks

**Module reflection**

- How are change and configuration management handled at your organization?

- Which of the treacherous 12 did you find the most interesting?

- How can incident response be improved at your organization?

---
