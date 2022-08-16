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

## Treacherous 12(1): Data Breaches
