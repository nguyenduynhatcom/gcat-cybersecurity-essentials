# Google Office of the CISO Institute: Cybersecurity Essentials

## Module 1: Introduction to Cybersecurity

### Inspect the CIA Triad: Confidentiality, Integrity, Availability
  | |Confidentiality|Integrity|Availability|
  | -------------------|----------------|--------|------------|
  |Example|Limit access by physical barriers or encryption|Perform an audit or a digital signature|Implement load balancing or backup data|
  |Attacks| Shoulder surf or sniff network data|Forge a signature or modify a spreadsheet trans|Perform a denial of service attack or install ransomware|

### Defend with Security Controls
  - Defending an organization requires control measure to be taken that strengthen security
  - The measures implemented vary according to:
    - The importance of the information and system
    - The assets to be protected
    - How the control functions
### Security control types
  ||Administrative|Technical|Physical|
  |---|---|---|---|
  |Who|Management|IT Specialist|Site and facilities personnel|
  |How|Creating policies and guides, as well as making decisions|Deploying technical defenses, such as endpoint security and firewalls, to defend against attacks|Implementing physical measures, such as guards and fences, to defend assets|

### Reasons for strong defenses
- Legal and regulatory mandates.
  |Example|Focus of control|
  |---|---|
  |PCI DSS|Payment card safety for customers. It is industry self-regulation.|
  |HIPAA|This US law covers the privacy and security of information handled by healthcare organizations.|
  |GDPR|European Union law that regulates the use or personal data|
  |FISMA|US law governing the control and structure of security for the government and contractors, requiring adherence to the Risk management framework by NIST|

- Violation costs
  |If a party is found to be in violations of rules, there are potentially large costs|Potential penalties for violations (July 2022) |
  |---|---|
  |PCI DSS|Fines of up to $100,000, increased monitoring, additional audits|
  |HIPAA|Fines of up to $50,000 per violation|
  |GDPR|GDPR allows fines of up to 11-22 million euros|


- Good business practices
- Bad actors seeking to find and exploit vulnerabilities

### Identify assets to protect

#### Organizational assets to defend
|Asset|Description|
|---|---|
|Data|Information stored, transmitted as well as used|
|End-user vehicles|Systems used by people|
|Servers|Systems that store and process information|
|Intranet|The internal networks|
|Perimeter networks|Networks placed just outside and intranet and accessed by the public|
|IoT|Small systems, such as home automation and automobiles, that perform specialized function|
|Cloud|Remote servers accessed over the internet| 

#### Data
Data is commonly viewed as existing in three states:
- Data in use
  - Information being used to process requests may face an array of threats of threats:
    - Eavesdropping
    - Modification
    - Destruction
  - For example, attackers may wish to misuse a SQL query to gain access to information. A common defense is to perform input validation before performing a transaction.

- Data at rest
  - Bad actors may seek to exfiltrate sensitive information using storage devices.
  - Parties with access could use:
    - A USB device
    - Stolen backups
    - Data remnants pilfered from discarded storage devices
  - Defensive measures could include sanitization, USB blockers, and encryption.

- Data in motion
  - Attackers may use network tools to intercept, monitor, or change information as moves using: 
    - Protocol analyzers
    - On-Path (Man-in-the-Middle) tools
    - Compromised network devices
  - Defenses generally include network access control and encryption.

- Special types of data
  - PII (Personally Identifiable Information or Personal Information): It can be private information or be used to identify a party directly or indirectly.
  - SPII (Special Personally Identifiable Information or Sensitive Data): Compromise could result in significant harm of a party.
  - PHI (Protected Health Information): HIPAA-defined health or personal information.

### End User Devices
#### End-user devices
These systems are generally for people.  
They may be:
- Dedicated to an individual
- Shared like a kiosk
- Mobile devices, portable systems or desktop computers.
- Printers and thermostats.

Attackers may deceive the user, steal the device, data stored on it or information on a server that is accessible by it.  
Endpoint defenses are deployed to defend them.

#### Servers
These are systems that may be centrally accessed. Commonly, they have larger storage and processing capabilities than workstations.
Bad actors seek them out because:
- Servers may have vast troves of valuable information
- They may be placed so that access by the public is allowed

Endpoint defenses and other specialized server application measures must be employed to defend them.

#### Intranet
"A computer network, especially one based on Internet technology, that an organization uses for its own internal (and usually private) purposes and that is closed to outsiders." - Internet Security Glossary, Version 2
Access by intruder could allow:
- Probes and attacks of sensitive internal resources
- Loss of trust by insiders

Defenses include physical measures, network access controls, firewalls, and authentication/authorization.

#### Perimeter networks
This is the outside network just beyond an organization’s intranet. Systems placed there are commonly available via the internet and may be accessible by the public.

This network and its systems face threats from:
- Nearly the entire internet
- Bad actors seeking to find a vector to reach the organization’s intranet

Defenses include firewalls, zero-trust network access, and filters.

#### Internet of Things
Small systems that are dedicated to particular tasks.

Examples include:

- Industrial control systems

- Home automation

- Building control systems and sensors

IoT devices are often controlled via edge and cloud-based servers.

These devices often have no defenses and may not have been designed with security in mind. Keeping them within a security perimeter is key.

#### Cloud
The cloud refers to a model for ubiquitous, convenient, on-demand access to pools of configurable computing that can be quickly provisioned and deprovisioned.

Shared multi-tenant facilities, as well as dedicated personnel, create a strong economy of scale. There are several procurement models. 

- Physical control and security is handled by the cloud service provider. 

- Logical control and security remain with the customer.

### Summary
#### Cybersecurity
Organizations must be dedicated to the protection of their data, systems, and networks.

#### The CIA Triad
The core of security principles is the CIA triad:

- Confidentiality
- Integrity
- Availability

#### Defensive Controls
To counter threats, controls are used to minimize or prevent exploitation. These may be administrative, technical, or physical measures.

#### Assets to Protect
While data is a key asset to protect, defenses must also be staged for user devices, servers, and IoT located from an intranet all the way out to the cloud.

## Module 2: Laws, Policies and Frameworks

### Module Objectives 
- Understand the need for laws, policies, and frameworks
- Recognize the functions of governance, risk, and compliance
- Identify key roles in cybersecurity
- Interpret important frameworks and standards for managing cybersecurity

"Putting data protection at the centre of digital businesses strategies is the key to improving trust and digital growth." - Steve Woods, Deputy Commisioner, ICO

### GRC in the organization
#### Governance, risk and compliance
This is the organizational stratefy for:
- Assigning responsibility
- Managing risk
- Ensuring compliance with policies, laws, and regulations

#### Governance
Governance determines control and responsibility. Those who control an asset are tasked with:
- Securing it
- Using it properly
- Implementing controls

#### Risk management
This organizational process oversees how risk is approached.
- Risk is inherent to any business, so it should be assessed.
- It should be managed in a way that it becomes acceptable.
- For example, a business may be worried about a power outage. A long outage would be unacceptable.
  - So they installed a backup generator.

This aspect of governance, risk, and compliance ensures an organization is using resources properly to counter unacceptable risks. 

#### Compliance

In today's complex world, organizations small and large face significant oversight.

Regulations and compliance may be:

- Voluntary
- Mandated by laws or industry regulations
- A unique policy of the organization

The compliance function seeks to ensure conformance, and prove the organization adheres to requirements.

### Cybersecurity roles and groups
#### Cybersecurity positions and roles
- Positions held by a party or a role
- These include:
  - Chief Information Security Officer
  - Security manager
  - Security engineer
  - Security analyst
  - Help desk
  - Developer and DBA
  - Legal department
  - Human resources
  - Blue team
  - Red team
  - Incident response team

#### Chief Information Security Officer (CISO)
The CISO has primary responsibility for ensuring the organization has proper security protections in place.

This includes:

- Governance, risk, and compliance
- Countering current threats
- Formulating strategies for the future

#### CISO and other senior officers
CISOs are primarily concerned with the overall data security of organization data on its systems
and networks. This commonly involves coordinating with or relying upon other senior officers.

- **Chief Privacy Officer** - tasked with protecting personal information and managing its
collection, storage, sharing, and transmission as well as seeing to compliance.

- **Chief Data Officer** - manages data-related functions that commonly include these aspects of
organization data: use and management, quality, and future data strategies.

- **Chief Information Officer** - handles the broad strategic planning of the organization
information technology initiatives. Depending on the organization, the CISO may or may not
report to this position.

#### Cybersecurity manager
This is an operational position. The tasks and functions of a cybersecurity manager include:

- Maintaining operational control over security activities
- Implementing and maintaining controls
- Conducting audits
- Investigating incidents
- Issuing reports
- Providing input to the CISO for strategy

#### Security engineer

A security engineer is a hands-on technical specialist.

They are typically specialized in particular procedures and software, such as:

- Implementing control measures
- Vulnerability assessment
- Firewall management

#### Security analyst

A security analyst is an IT specialist who specializes in monitoring, implementing procedures and research.

Their responsibilities may include:

- Intrusion monitoring
- Incident investigation
- Risk assessment
- Verify patching and remediation
- Threat research

#### Help desk

Help desk personnel perform several key functions in security.

They are often the first responder to security incidents. They have these key functions regarding security incidents:

- Performing triage when a significant disruption occurs.
- Communicating with users
- Performing account maintenance
- Initial isolation of an incident or crime scene
- Implementing specific procedures and fixes

#### Developers and DBA

Developers and database administrators often work together and have shared areas of expertise in applications and security.

Particularly with web applications, it is useful to have the capabilities, knowledge, and skills when:

- A breach occurs
- Vulnerability is discovered
- Misuse of application privileges is suspected

#### Legal department

The legal department can help ensure that incident handling and responses are done properly according to:

- Industry regulations
- Laws
- Organization policy

Legal counsel is especially important when criminal or significant liability issues are in play.

- Data breach
- Theft or other misuse
- Contractual obligations

#### Human resources

The HR role is typically to provide guidance during incidents where employees:

- Are the subject of an investigation
- Have become the victims
- Failed to perform their duties properly

In many organizations, it is HR that must take certain actions, such as dismissal, retraining, or reassignment.

#### Blue team

Members of this team fulfill a role. It is not a specific position.

These personnel maintain defenses. The members may work together on projects requiring broad knowledge and multiple disciplines

Typical membership includes:

- Security engineer
- Security analyst
- Help desk
- Developers and DBA

#### Red team

Members of this team also fulfill a role.

These personnel perform security testing, such as penetration tests. It is common for these team members to be contracted from outside an organization for specific jobs.

Typical skills include:

- Hacking
- Social engineering
- Scanning and reconnaissance

They may be pitted against a blue team to assess operational security.

#### Incident response teams

A variety of incident response teams may be created for differing incidents. The staffing is dictated by the kind of issue or incident, such as:

- Malware on a single machine
- Data breach of sensitive customer data
- Rogue user actions in an application

### Managing Risks

#### Managing Risks

Risk is inherent to any activity.

Some activities are riskier than others:
- Manufacturing explosives
- Performing transactions over the Internet

It is important to identify risks and reduce them when something is seen as too risky.

An organization that does not know its risks has little ability to control them.

#### Handling Risk

There are four ways to address risk:

- **Accept** - when the risk is identified and assessed to be within the organization's risk tolerance.
- **Mitigate** - excessive risk is reduced to a level of acceptability.
- **Transfer** - impact is shared or shifted to a third party, such as insurance.
- **Avoid** - cancel or eliminate when risk is excessive or beyond the organization's risk tolerance.

After all has been done, residual risk is always present.

### Match the terms


| Term | Example or Description |
|---|---|
| **Risk management** | Properly countering unacceptable risks |
| Blue team | These personnel maintain defenses |
| Security Analyst | Specialists in security monitoring, investigating incidents, and research |
| Compliance | Adhering to laws and policies |
| **Categorize** | Identifying the importance of a system and its information |
| Select | Tailor controls for unique requirements |


### Commonly Used Frameworks and Standards 

#### Security frameworks and regulations


#### PCI-DSS 

#### ISO 27000 series 

#### CIS Controls

#### NIST Cybersecurity Framework

#### DISA STIGs

#### HIPAA 

#### Federal Risk and Authorization Management Program (FedRAMP)

#### Cloud Controls Matrix 

### Risk Management Framework steps

This is the NIST RMF. There are other models for managing risk.

| Step | Description |
|---|---|
| Prepare | Carry out preliminary activities. |
| Categorize | Assign and record security requirements and system characteristics. |
| Select | Choose the appropriate controls. |
| Implement | Deploy the controls. |
| Assess | Verify controls are performing as expected. |
| Authorize | Take responsibility, if the risk is acceptable. |
| Monitor | Continuously check the asset and update its status. |

#### Prepare

Whether it is a new system or an organizational activity, the first step is to become aware of the potential issues, defenses, and acceptable risk levels.

- Identify assets and risks to be assessed and managed.
- Determine risk tolerance.
- Discover common controls and defenses already present.

#### Categorize

Determining the negative impacts of potential breaches and security requirements of confidentiality, integrity, and availability of information and systems. Not all systems have the same requirement for each element of CIA.

These security characteristics should be based upon:

- The importance and use of the system
- The information processed, as well as the information stored and transmitted

#### Select

Based upon the risk tolerance and the security characteristics of the system, these decisions are made:

- Determine the controls needed to achieve acceptable security
- Tailor controls for unique requirements
- Identify the proper monitoring to be performed
- Discover any unique or system-specific security requirements
- Develop an ongoing security plan

#### Implement

Risk controls are implemented. This can be done by:

- Using the common environment; e.g., using site physical security to defend against fire and theft
- Integrating controls into the system itself; e.g., implementing input validation in a web application
- Bolt-on components, which are external to the system that achieve the needed security. This is the least desirable means.

These controls are recorded in a system record and a risk register.

#### Assess

Based upon previous steps, independent parties assess the effectiveness of the controls and plans.

- Monitoring plans are reviewed
- Controls tested
- Deficiencies reports created
- Remediation actions are planned and implemented
- Status updated to reflect changes and remediation

A recommendation is made as to whether risk is acceptable.

#### Authorize

Responsibility is taken for the system. A party in the organization who knows the characteristics, use, controls implemented and assessments make a decision. It may be:

- Approved
- Denied
- Given interim or temporary approval

The authorizing official may accept or reject the recommendation of the assessors. The decision may also be referred upward to a higher level officer in an organization.

#### Monitor

Implement processes that periodically or continuously assess:

- Vulnerabilities that relate to the asset
- Controls effectiveness
- News in the threat landscape
- Changes in the use or purpose of the asset




### Law Policies Frameworks Quiz

#### Question 1
What are the first steps in managing risk?

A. Performing a comprehensive personnel assessment.

B. Examining threat feeds and determining likely points of attack.

**C.** Asset and risk identification.

D. Decommissioning high-risk systems.

#### Question 2
Vị trí an ninh mạng nào phụ trách hoạt động an ninh hàng ngày?
A. Nhà phân tích cấp cao thường được giao phụ trách các hoạt động hàng ngày.

B. Giám đốc An toàn Thông tin có nhiệm vụ này.

C. Kỹ sư bảo mật giám sát hoạt động hàng ngày; Các nhà phân tích xử lý các chiến lược.

**D.** Trình quản lý an ninh mạng giám sát các hoạt động bảo mật.

#### Question 3
What is a military guide that identifies need remediation?
**A.** STIG: Security Technical Implementation Guide

B. CVE Common Vulnerabilities and Exposures Entries with critical scores

C. CIS Control Alerts 

D. Cloud Control Matrix Notices


#### Question 4
What is the US Federal Program that oversees the adoption and use of cloud services?

A. PCI-DSS Cloud Controls Requirements which is industry self-regulation.

**B.** FedRAMP: Federal Risk and Authorization Management Program

C. NIST Special Publications Group for FISMA Cloud Compliance 

D. Cloud Control Matrix - Federal Division

### Module Summary