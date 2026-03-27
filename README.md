# FISMA Compliance Checklist

A comprehensive compliance checklist, readiness guide, and control mapping for organizations subject to the Federal Information Security Modernization Act (FISMA). This repository covers the NIST standards mandate, annual reporting requirements, Inspector General assessments, CISA oversight, and the Risk Management Framework (RMF) process.

Last Reviewed: March 2026

## Table of Contents

- [What Is FISMA?](#what-is-fisma)
- [FISMA Legislative History and Evolution](#fisma-legislative-history-and-evolution)
- [Who Must Comply with FISMA?](#who-must-comply-with-fisma)
- [Relationship to NIST SP 800-53 and the RMF](#relationship-to-nist-sp-800-53-and-the-rmf)
- [FISMA Key Requirements](#fisma-key-requirements)
- [CISA Oversight and Reporting](#cisa-oversight-and-reporting)
- [Inspector General Assessments](#inspector-general-assessments)
- [FISMA Metrics and Scoring](#fisma-metrics-and-scoring)
- [FISMA Compliance Checklist](#fisma-compliance-checklist-1)
- [Common Compliance Gaps](#common-compliance-gaps)
- [How PTG Helps with FISMA Compliance](#how-ptg-helps-with-fisma-compliance)
- [Frequently Asked Questions](#frequently-asked-questions)
- [Additional Resources](#additional-resources)

## What Is FISMA?

The Federal Information Security Modernization Act (FISMA) is a United States federal law that establishes a comprehensive framework for securing federal government information, operations, and assets against natural or man-made threats. Originally enacted in 2002 as the Federal Information Security Management Act and updated in 2014 as the Federal Information Security Modernization Act, FISMA mandates that every federal agency develop, document, and implement an agency-wide information security program.

FISMA is codified at 44 U.S.C. 3551-3558 and assigns specific responsibilities across the federal government. The Office of Management and Budget (OMB) oversees implementation and provides policy guidance. The Cybersecurity and Infrastructure Security Agency (CISA) within the Department of Homeland Security provides operational cybersecurity support and issues binding operational directives. The National Institute of Standards and Technology (NIST) develops the security standards and guidelines that agencies must follow. Agency heads are ultimately responsible for their organization's information security posture.

The practical impact of FISMA extends well beyond federal agencies themselves. Any organization that processes, stores, or transmits federal information, or operates information systems on behalf of a federal agency, must comply with FISMA requirements. This includes federal contractors, grantees, state agencies administering federal programs, and cloud service providers hosting federal data.

FISMA compliance is not optional. The Federal Information Security Modernization Act gives OMB the authority to enforce compliance, and agency Inspector Generals conduct annual independent evaluations. Agencies that fail to meet FISMA requirements face budget impacts, unfavorable Congressional oversight, and in severe cases, restrictions on IT spending authority.

## FISMA Legislative History and Evolution

Understanding FISMA's evolution provides important context for its current requirements:

**2002: Original FISMA (FISMA 2002).** The Federal Information Security Management Act of 2002 was enacted as Title III of the E-Government Act. It established the initial framework for federal information security, directed NIST to develop security standards, and required annual agency reporting.

**2014: FISMA Reform (FISMA 2014).** The Federal Information Security Modernization Act of 2014 updated the original law to reflect the evolved threat landscape. Key changes included elevating CISA's role (then NPPD) in operational cybersecurity, shifting from paper-based compliance to real-time monitoring, requiring automated security monitoring tools, and streamlining reporting requirements.

**2023: FISMA Update Proposals.** Congressional efforts to further modernize FISMA have focused on codifying zero trust architecture requirements, mandating incident reporting timelines, strengthening supply chain risk management, and improving coordination between agencies and CISA.

**2024-2025: OMB Memoranda.** OMB has issued updated guidance reinforcing zero trust adoption timelines, cloud security requirements, and AI security considerations under the FISMA framework.

## Who Must Comply with FISMA?

FISMA compliance requirements apply to a broad range of organizations:

**Federal Executive Branch Agencies.** All cabinet departments, independent agencies, and government corporations must comply with FISMA.

**Federal Contractors.** Organizations that operate information systems on behalf of federal agencies or process federal information under contract must implement FISMA-required controls. This is typically enforced through contract clauses referencing NIST SP 800-171 for Controlled Unclassified Information (CUI) or NIST SP 800-53 for systems that directly support federal operations.

**State and Local Agencies.** State and local government entities that administer federal programs (such as Medicaid, SNAP, or federal education programs) must protect federal information in accordance with FISMA requirements.

**Cloud Service Providers.** CSPs hosting federal data must achieve FedRAMP authorization, which implements NIST SP 800-53 controls as required by FISMA.

**Grantees.** Organizations receiving federal grants that involve access to federal information systems or data may be subject to FISMA requirements as a condition of the grant.

**Research Institutions.** Universities and research organizations with federal contracts or grants involving sensitive data must comply with applicable FISMA requirements.

## Relationship to NIST SP 800-53 and the RMF

FISMA mandates that federal agencies follow NIST security standards and guidelines. This creates a direct dependency chain:

**NIST SP 800-53 Rev. 5** is the comprehensive catalog of over 1,000 security and privacy controls organized into 20 families. FISMA requires agencies to implement controls from this catalog based on the impact level (Low, Moderate, or High) of each information system.

**NIST SP 800-37 Rev. 2 (Risk Management Framework)** defines the six-step process agencies must follow to manage security risk:

1. **Categorize** the information system (using FIPS 199 and NIST SP 800-60)
2. **Select** security controls (from NIST SP 800-53, refined by NIST SP 800-53B baselines)
3. **Implement** the selected security controls
4. **Assess** control effectiveness (following NIST SP 800-53A)
5. **Authorize** the system to operate (formal risk acceptance by the Authorizing Official)
6. **Monitor** security controls on an ongoing basis

**FIPS 199** establishes the security categorization of federal information and information systems based on potential impact: Low, Moderate, or High.

**FIPS 200** specifies the minimum security requirements for federal information and information systems across 17 security-related areas.

**NIST SP 800-53B** defines the control baselines (Low, Moderate, High) that determine which SP 800-53 controls apply at each impact level.

This hierarchy means FISMA compliance is, in practice, NIST SP 800-53 compliance implemented through the Risk Management Framework. Organizations already implementing NIST controls for other frameworks (CMMC, FedRAMP, StateRAMP, HIPAA via SP 800-66) can leverage that work directly toward FISMA compliance.

For the official NIST SP 800-53 publication, visit [https://csrc.nist.gov/publications/detail/sp/800-53/rev-5/final](https://csrc.nist.gov/publications/detail/sp/800-53/rev-5/final).

For the NIST Risk Management Framework, visit [https://csrc.nist.gov/projects/risk-management/about-rmf](https://csrc.nist.gov/projects/risk-management/about-rmf).

## FISMA Key Requirements

FISMA establishes several core requirements for federal information security:

### 1. Agency-Wide Information Security Program

Each agency must develop, document, and implement an information security program that includes:

- Periodic risk assessments of the risk and magnitude of harm from unauthorized access, use, disclosure, disruption, modification, or destruction of information systems
- Risk-based policies and procedures that adequately reduce risks to an acceptable level
- Subordinate plans for providing adequate security for networks, facilities, and systems
- Security awareness training for personnel (including contractors)
- Testing and evaluation of security controls with frequency based on risk
- Remediation of deficiencies
- Procedures for detecting, reporting, and responding to security incidents
- Plans and procedures for continuity of operations

### 2. System Security Categorization

Agencies must categorize every information system using FIPS 199 criteria based on the potential impact of a security breach on confidentiality, integrity, and availability. The system is categorized at the highest impact level of any information type it processes.

### 3. Risk Management Framework Execution

Agencies must apply the NIST Risk Management Framework to every information system, ensuring that security controls are selected, implemented, assessed, authorized, and monitored according to the system's risk profile.

### 4. Annual Reporting

FISMA requires agencies to report annually to OMB on the status of their information security programs. Reports must include:

- System inventory and categorization
- Security control assessment results
- Plan of Action and Milestones (POA&M) status
- Continuous monitoring status
- Incident statistics and response metrics
- Training compliance data

### 5. Inspector General Evaluation

Each agency's Inspector General (or independent external auditor) must conduct an annual independent evaluation of the agency's information security program and practices. This evaluation assesses:

- Compliance with FISMA requirements
- Effectiveness of security controls
- Adherence to NIST standards
- Incident response capabilities
- Progress on remediation of known vulnerabilities

### 6. Continuous Monitoring

FISMA 2014 emphasized the shift from annual compliance snapshots to continuous monitoring, requiring agencies to implement automated tools that provide near-real-time visibility into their security posture.

## CISA Oversight and Reporting

The Cybersecurity and Infrastructure Security Agency (CISA) plays a central operational role in FISMA implementation:

**Binding Operational Directives (BODs).** CISA issues binding directives that require agencies to take specific cybersecurity actions within defined timeframes. Examples include BOD 22-01 (Reducing the Significant Risk of Known Exploited Vulnerabilities) and BOD 23-01 (Improving Asset Visibility and Vulnerability Detection).

**Emergency Directives.** When active exploitation or imminent threats are identified, CISA issues emergency directives requiring agencies to take immediate action, such as patching critical vulnerabilities or isolating compromised systems.

**CDM Program.** The Continuous Diagnostics and Mitigation (CDM) program provides agencies with tools, integration services, and dashboards to strengthen their security posture and provide CISA with near-real-time visibility.

**Incident Reporting.** Agencies must report security incidents to CISA's US-CERT within defined timeframes based on incident severity. Major incidents require Congressional notification.

**FISMA CIO Metrics.** CISA coordinates the annual FISMA CIO metrics collection, which measures agency performance across eight domains: Identify, Protect, Detect, Respond, Recover, Supply Chain Risk Management, Privacy, and Cross-Agency Priority Goals.

**Threat Intelligence.** CISA provides agencies with threat intelligence, vulnerability alerts, and cybersecurity advisories that feed into agency risk management processes.

## Inspector General Assessments

The IG evaluation is one of the most consequential elements of FISMA compliance:

### IG Evaluation Domains

Inspector General assessments evaluate agencies across domains aligned with the NIST Cybersecurity Framework:

**Identify.** Risk management, asset management, governance, supply chain risk management.

**Protect.** Identity management and access control, awareness and training, data security, information protection processes, maintenance, protective technology.

**Detect.** Anomalies and events, security continuous monitoring, detection processes.

**Respond.** Response planning, communications, analysis, mitigation, improvements.

**Recover.** Recovery planning, improvements, communications.

### IG Maturity Model

IG assessments rate agencies using a maturity model with five levels:

1. **Ad Hoc:** Policies and procedures are not formalized; activities are performed in a reactive manner.
2. **Defined:** Policies and procedures are formalized and documented but not consistently implemented.
3. **Consistently Implemented:** Policies and procedures are consistently implemented but quantitative and qualitative effectiveness measures are lacking.
4. **Managed and Measurable:** Quantitative and qualitative measures on the effectiveness of policies and procedures exist and are used to improve security.
5. **Optimized:** Policies and procedures are fully institutionalized, regularly updated, and proactively address evolving threats.

Agencies at Level 4 (Managed and Measurable) or above are generally considered to have an effective information security program.

### Common IG Findings

Based on publicly available IG reports, the most common findings include:

- Incomplete system inventories
- Outdated or missing system security plans
- Inadequate configuration management
- Insufficient continuous monitoring
- Overdue POA&M items
- Incomplete security awareness training
- Weak identity and access management controls

## FISMA Metrics and Scoring

OMB and CISA collect FISMA metrics from agencies to assess the overall cybersecurity posture of the federal government:

### CIO Metrics (Self-Reported)

Agencies report metrics across eight domains, with questions designed to measure the maturity and effectiveness of specific security capabilities. Metrics are scored using the same five-level maturity model used by IGs.

### Cross-Agency Priority (CAP) Goals

FISMA metrics align with government-wide cybersecurity CAP goals, which have included:

- Increasing adoption of endpoint detection and response (EDR) tools
- Achieving specific MFA deployment percentages
- Encrypting data at rest and in transit
- Implementing zero trust architecture milestones
- Improving vulnerability remediation timelines

### Federal Cybersecurity Scorecard

OMB publishes the Federal Cybersecurity Scorecard based on FISMA metrics and IG evaluations. Agencies receive grades that are visible to Congress and the public, creating accountability pressure.

## FISMA Compliance Checklist

See the full detailed checklist in [compliance-checklist.md](compliance-checklist.md).

A summary of the major compliance areas:

### Program-Level Requirements
- [ ] Establish agency-wide information security program
- [ ] Designate Chief Information Security Officer (CISO)
- [ ] Develop and maintain enterprise security architecture
- [ ] Conduct annual agency risk assessment
- [ ] Report annually to OMB per FISMA requirements
- [ ] Support Inspector General annual evaluation

### System-Level Requirements
- [ ] Categorize all information systems per FIPS 199
- [ ] Execute RMF for every information system
- [ ] Maintain current System Security Plans (SSPs)
- [ ] Implement NIST SP 800-53 controls per impact level
- [ ] Conduct security control assessments per NIST SP 800-53A
- [ ] Obtain and maintain Authorization to Operate (ATO)
- [ ] Implement continuous monitoring program

### Operational Requirements
- [ ] Deploy automated monitoring tools (CDM or equivalent)
- [ ] Implement SIEM for security event correlation
- [ ] Report incidents to CISA/US-CERT per reporting timelines
- [ ] Maintain and update Plan of Action and Milestones (POA&M)
- [ ] Conduct monthly vulnerability scanning
- [ ] Complete annual penetration testing
- [ ] Provide security awareness training to all personnel

### Identity and Access Management
- [ ] Implement multi-factor authentication (MFA)
- [ ] Deploy privileged access management (PAM) solution
- [ ] Maintain complete user account inventory
- [ ] Enforce least privilege access
- [ ] Implement role-based access controls

### Data Protection
- [ ] Encrypt data at rest using FIPS 140-2 validated modules
- [ ] Encrypt data in transit using FIPS 140-2 validated modules
- [ ] Implement data loss prevention (DLP) controls
- [ ] Classify and label sensitive information
- [ ] Implement media sanitization procedures per NIST SP 800-88

## Common Compliance Gaps

Based on 23+ years of cybersecurity experience, these are the most frequently encountered FISMA compliance gaps:

1. **Incomplete System Inventories.** Agencies and contractors struggle to maintain accurate, comprehensive inventories of all information systems, particularly when cloud services, shadow IT, and contractor-operated systems are involved.

2. **Stale Authorizations.** Systems operating on expired ATOs or with significant changes since their last authorization. FISMA requires ongoing authorization, not one-time approval.

3. **Insufficient Continuous Monitoring.** Paper-based compliance that fails to detect real-time threats. FISMA 2014 specifically addressed this gap by mandating automated, continuous monitoring.

4. **POA&M Backlogs.** Large numbers of overdue remediation items in the Plan of Action and Milestones, indicating systemic inability to address known vulnerabilities.

5. **Weak Identity Management.** Incomplete MFA deployment, orphaned accounts, excessive privileged access, and lack of privileged access management tools.

6. **Configuration Management Drift.** Systems that deviate from approved baseline configurations without proper change control documentation.

7. **Contractor Oversight.** Insufficient visibility into how contractors implement security controls for systems operated on behalf of federal agencies.

8. **Supply Chain Risk.** Inadequate assessment and monitoring of risks introduced through the hardware and software supply chain.

## How PTG Helps with FISMA Compliance

Petronella Technology Group, Inc. (PTG) provides comprehensive FISMA compliance services for federal contractors, grantees, and organizations that process federal information.

### Craig Petronella's Credentials

Every PTG engagement is led by Craig Petronella, whose qualifications include:

- **CMMC Registered Practitioner**, qualified to conduct CMMC assessments for defense contractors
- **Licensed Digital Forensic Examiner #604180**, providing forensic investigation capabilities when security incidents occur
- **Cisco CCNA and CWNE**, demonstrating deep networking and wireless security expertise
- **MIT Artificial Intelligence Certificate**, combining AI knowledge with cybersecurity
- **Amazon #1 Best-Selling Author** of 14+ cybersecurity books
- **23+ years in cybersecurity**, with hands-on experience across federal compliance frameworks

### What Makes PTG Different

**AI-Powered Compliance.** PTG uses its own private AI fleet, including on-premise large language models and custom GPU infrastructure, to accelerate compliance assessments, automate control mapping, and continuously monitor security posture. No other firm in the Research Triangle has this capability.

**Patented Technology Stack.** PTG's proprietary, patented security and compliance tools automate what competitors do manually, reducing assessment timelines and improving accuracy across the entire RMF lifecycle.

**Licensed Digital Forensic Examiner.** When compliance fails and a breach occurs, PTG has the forensic expertise to investigate, preserve evidence, and support legal proceedings. Most compliance firms cannot offer this, which is critical for FISMA incident response requirements.

**AI + Cybersecurity Combined.** PTG is one of the only firms that combines AI development (custom AI agents, private LLMs, GPU hosting) with cybersecurity and compliance. As federal agencies adopt AI systems, FISMA compliance must extend to AI-specific risks, and PTG is uniquely positioned to address both.

**Fleet Infrastructure.** PTG's on-premise AI infrastructure (GPU clusters, private cloud) proves PTG practices what it preaches about data sovereignty and private AI, which is directly relevant to agencies concerned about data sovereignty.

**SMB Focus.** PTG makes enterprise-grade FISMA compliance accessible to small and mid-size federal contractors and grantees who need the same rigor as large systems integrators but at a scale and price point that works for their organization.

### Services for FISMA

PTG provides end-to-end FISMA compliance services:

- **System Categorization**: FIPS 199 categorization of information systems and data types
- **Gap Assessment**: Comprehensive evaluation against NIST SP 800-53 control baselines
- **RMF Execution**: Full Risk Management Framework implementation support
- **SSP Development**: Complete System Security Plan authoring and documentation
- **Assessment Support**: Preparation for and support during IG evaluations
- **Continuous Monitoring**: AI-powered continuous monitoring services
- **Incident Response**: 24/7 incident response with forensic capabilities for CISA reporting requirements
- **POA&M Management**: Ongoing tracking and remediation of security findings

**Ready to strengthen your FISMA compliance posture?** Call 919-348-4912 or visit [https://www.petronellatech.com/compliance/fisma/](https://www.petronellatech.com/compliance/fisma/) to schedule a free compliance assessment.

See also: [PTG Compliance Packages](https://www.petronellatech.com/compliance/packages/)

## Frequently Asked Questions

**Q: Who enforces FISMA?**
A: FISMA enforcement involves multiple entities. OMB provides policy oversight and guidance. CISA provides operational cybersecurity support and issues binding operational directives. Agency heads are responsible for their organization's compliance. Agency Inspector Generals conduct independent annual evaluations. Congress exercises oversight through committee hearings and budget processes.

**Q: Does FISMA apply to contractors?**
A: Yes. FISMA requirements flow down to federal contractors through contract clauses, particularly FAR 52.204-21 (basic safeguarding) and DFARS 252.204-7012 (for defense contractors). Contractors operating information systems on behalf of federal agencies or processing federal information must implement appropriate NIST controls.

**Q: What is the difference between FISMA and FedRAMP?**
A: FISMA is the law that mandates federal information security programs and requires adherence to NIST standards. FedRAMP is a program that implements FISMA requirements specifically for cloud service providers used by federal agencies. FedRAMP uses NIST SP 800-53 controls (as required by FISMA) plus additional cloud-specific parameters.

**Q: How does FISMA relate to CMMC?**
A: FISMA requires implementation of NIST SP 800-53 controls for federal information systems. CMMC requires implementation of NIST SP 800-171 controls (a subset of SP 800-53 Moderate baseline tailored for CUI) for defense contractors. Both derive from the same NIST control catalog. Organizations subject to both can leverage overlapping controls.

**Q: What are the penalties for FISMA non-compliance?**
A: FISMA does not prescribe specific fines, but consequences include reduced cybersecurity scores visible to Congress and the public, OMB budget restrictions on IT spending, negative IG findings in annual evaluations, potential loss of federal contracts for non-compliant contractors, and Congressional oversight hearings.

**Q: How often must FISMA assessments be conducted?**
A: FISMA requires continuous monitoring, with specific periodic activities including monthly vulnerability scanning, annual security control assessments, annual IG evaluations, and annual reporting to OMB. Additionally, assessments are required whenever significant changes occur to information systems.

**Q: What is the relationship between FISMA and NIST SP 800-171?**
A: FISMA requires agencies to follow NIST standards for securing federal information. NIST SP 800-53 applies to federal information systems directly. NIST SP 800-171 was derived from SP 800-53 to define requirements for protecting Controlled Unclassified Information (CUI) in non-federal systems, such as contractor environments. Both are rooted in the same NIST SP 800-53 master control catalog.

**Q: How does zero trust architecture fit into FISMA?**
A: OMB Memorandum M-22-09 requires federal agencies to achieve specific zero trust architecture goals, and these requirements are enforced within the FISMA framework. Zero trust principles, including "never trust, always verify," micro-segmentation, and continuous validation, are increasingly integrated into FISMA metrics and IG evaluations. NIST SP 800-207 provides the reference architecture for federal zero trust implementation.

## Additional Resources

- [FISMA (44 U.S.C. 3551-3558)](https://www.govinfo.gov/app/details/USCODE-2018-title44/USCODE-2018-title44-chap35-subchapII)
- [NIST SP 800-53 Rev. 5](https://csrc.nist.gov/publications/detail/sp/800-53/rev-5/final)
- [NIST SP 800-37 Rev. 2 (Risk Management Framework)](https://csrc.nist.gov/publications/detail/sp/800-37/rev-2/final)
- [NIST Cybersecurity Framework 2.0](https://www.nist.gov/cyberframework)
- [CISA Federal Cybersecurity](https://www.cisa.gov/topics/cybersecurity-best-practices/federal-cybersecurity)
- [OMB FISMA Reports](https://www.whitehouse.gov/omb/management/egov/)
- [PTG Compliance Services](https://www.petronellatech.com/compliance/)
- [PTG NIST Compliance](https://www.petronellatech.com/nist/)
- [PTG AI Services](https://www.petronellatech.com/ai/)
- [PTG Cybersecurity Services](https://www.petronellatech.com/cybersecurity/)
- [PTG Managed IT Services](https://www.petronellatech.com/managed-it/)

## About Petronella Technology Group, Inc.

Petronella Technology Group, Inc. (PTG) provides AI-powered cybersecurity and compliance services for small and mid-size businesses. Led by Craig Petronella, a CMMC Registered Practitioner, Licensed Digital Forensic Examiner (#604180), and Amazon #1 Best-Selling Author of 14+ cybersecurity books, PTG combines 23+ years of cybersecurity experience with cutting-edge AI technology to make enterprise-grade compliance accessible to organizations of all sizes.

**Petronella Technology Group, Inc.**
5540 Centerview Dr. Suite 200
Raleigh, NC 27606
Phone: 919-348-4912

[https://www.petronellatech.com](https://www.petronellatech.com)

## License

This checklist is provided under the MIT License. See [LICENSE](LICENSE) for details.
