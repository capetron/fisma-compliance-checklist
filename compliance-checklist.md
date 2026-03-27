# FISMA Compliance Checklist

A detailed, actionable checklist for organizations subject to the Federal Information Security Modernization Act (FISMA). Organized by the NIST Risk Management Framework steps and NIST SP 800-53 control families.

Last Reviewed: March 2026

## How to Use This Checklist

1. Identify whether you are a federal agency, contractor, grantee, or other covered entity.
2. Determine the FIPS 199 impact level (Low, Moderate, High) of each information system.
3. Work through each section, marking requirements as complete, in progress, or not started.
4. For incomplete items, document the gap and add to your Plan of Action and Milestones (POA&M).
5. Prepare for Inspector General evaluation by ensuring documentation is current and evidence is readily available.

Impact levels are indicated as follows:
- **[L]** = Required for Low impact systems
- **[M]** = Required for Moderate impact systems
- **[H]** = Required for High impact systems

If no level is specified, the requirement applies to all impact levels.

---

## 1. Program-Level Requirements (Agency-Wide)

### Governance
- [ ] Designate a Chief Information Security Officer (CISO) with authority and resources
- [ ] Establish an information security governance structure with clear roles and responsibilities
- [ ] Develop an agency-wide information security strategic plan
- [ ] Define risk tolerance and risk management strategy
- [ ] Establish policy review and update cadence (at least annually)
- [ ] Maintain enterprise-wide security architecture
- [ ] Integrate information security into capital planning and investment control (CPIC)

### System Inventory
- [ ] Maintain a comprehensive inventory of all agency information systems
- [ ] Identify system owners, authorizing officials, and security contacts for each system
- [ ] Document system boundaries, interfaces, and interconnections
- [ ] Categorize all systems per FIPS 199
- [ ] Track authorization status (ATO, IATT, DATO) for all systems
- [ ] Identify and document cloud services (IaaS, PaaS, SaaS) in use
- [ ] Track contractor-operated systems and third-party services

### Annual Reporting
- [ ] Submit annual FISMA report to OMB per CyberScope/FISMA metrics
- [ ] Support Inspector General annual evaluation
- [ ] Report FISMA CIO metrics across all eight domains
- [ ] Track and report Cross-Agency Priority (CAP) goal progress
- [ ] Report supply chain risk management maturity
- [ ] Report privacy program metrics
- [ ] Document corrective actions for IG findings

### Incident Management Program
- [ ] Establish agency incident response team or contract for IR services
- [ ] Define incident categories and severity levels
- [ ] Establish CISA/US-CERT reporting procedures and timelines
- [ ] Implement capability to detect, analyze, and respond to incidents
- [ ] Conduct annual incident response exercises
- [ ] Maintain incident tracking and after-action reporting
- [ ] Report major incidents to Congress within 7 days

## 2. Risk Management Framework (RMF) Execution

### Step 1: Categorize
- [ ] Identify all information types processed by the system (per NIST SP 800-60)
- [ ] Determine potential impact for each information type across confidentiality, integrity, availability
- [ ] Assign system categorization at the highest impact level (FIPS 199)
- [ ] Document categorization rationale
- [ ] Obtain authorizing official concurrence on categorization
- [ ] Record categorization in system security plan and system inventory

### Step 2: Select Controls
- [ ] Identify applicable NIST SP 800-53B baseline (Low, Moderate, or High)
- [ ] Apply scoping guidance to tailor controls to system environment
- [ ] Select additional controls based on risk assessment findings
- [ ] Document control selections in the system security plan
- [ ] Identify common controls provided by the organization or inherited from other systems
- [ ] Document hybrid controls with shared implementation responsibilities
- [ ] Identify compensating controls where standard controls cannot be implemented

### Step 3: Implement Controls
- [ ] **[L/M/H]** Implement all selected controls from the applicable baseline
- [ ] Document control implementations in the system security plan
- [ ] Implement controls across all 20 NIST SP 800-53 control families (see below)
- [ ] Configure systems per approved baseline configurations (STIG, CIS Benchmarks)
- [ ] Deploy required security tools (EDR, SIEM, vulnerability scanners, MFA)
- [ ] Implement FIPS 140-2 validated encryption for data at rest and in transit
- [ ] Deploy network segmentation and boundary protection

### Step 4: Assess Controls
- [ ] Develop security assessment plan per NIST SP 800-53A
- [ ] Engage independent assessors (for Moderate and High systems)
- [ ] Conduct security control assessment using approved assessment procedures
- [ ] Document assessment findings in Security Assessment Report (SAR)
- [ ] Identify findings as satisfied, partially satisfied, or other than satisfied
- [ ] Create POA&M entries for all findings not fully satisfied
- [ ] Perform remediation and reassess failed controls

### Step 5: Authorize
- [ ] Compile authorization package (SSP, SAR, POA&M)
- [ ] Present risk posture to authorizing official
- [ ] Authorizing official makes risk-based authorization decision
- [ ] Issue Authorization to Operate (ATO), Denial of ATO, or Interim ATO
- [ ] Document authorization decision and any conditions
- [ ] Communicate authorization decision to relevant stakeholders
- [ ] Set authorization expiration (typically 3 years, with continuous monitoring)

### Step 6: Monitor
- [ ] Implement continuous monitoring strategy per NIST SP 800-137
- [ ] Deploy automated monitoring tools (CDM program or equivalent)
- [ ] Conduct monthly vulnerability scanning
- [ ] Perform annual security control assessments
- [ ] Update SSP to reflect system changes
- [ ] Maintain and update POA&M
- [ ] Report monitoring status per agency and FISMA requirements
- [ ] Reassess authorization when significant changes occur

## 3. NIST SP 800-53 Control Family Checklist

### Access Control (AC)
- [ ] **[L/M/H]** AC-1: Access control policy and procedures
- [ ] **[L/M/H]** AC-2: Account management
- [ ] **[M/H]** AC-2(1): Automated account management
- [ ] **[M/H]** AC-2(2): Automated temporary/emergency account management
- [ ] **[M/H]** AC-2(3): Disable inactive accounts
- [ ] **[H]** AC-2(4): Automated audit actions
- [ ] **[L/M/H]** AC-3: Access enforcement
- [ ] **[M/H]** AC-4: Information flow enforcement
- [ ] **[L/M/H]** AC-5: Separation of duties
- [ ] **[L/M/H]** AC-6: Least privilege
- [ ] **[M/H]** AC-6(1-10): Least privilege enhancements
- [ ] **[L/M/H]** AC-7: Unsuccessful logon attempts
- [ ] **[L/M/H]** AC-8: System use notification
- [ ] **[M/H]** AC-10: Concurrent session control
- [ ] **[L/M/H]** AC-11: Session lock
- [ ] **[L/M/H]** AC-14: Permitted actions without identification
- [ ] **[L/M/H]** AC-17: Remote access
- [ ] **[M/H]** AC-17(1-4): Remote access enhancements
- [ ] **[L/M/H]** AC-18: Wireless access
- [ ] **[L/M/H]** AC-19: Mobile device access
- [ ] **[L/M/H]** AC-20: External system use
- [ ] **[M/H]** AC-21: Information sharing
- [ ] **[L/M/H]** AC-22: Publicly accessible content

### Awareness and Training (AT)
- [ ] **[L/M/H]** AT-1: Policy and procedures
- [ ] **[L/M/H]** AT-2: Security awareness training (including phishing)
- [ ] **[M/H]** AT-2(2): Insider threat awareness
- [ ] **[L/M/H]** AT-3: Role-based security training
- [ ] **[L/M/H]** AT-4: Training records

### Audit and Accountability (AU)
- [ ] **[L/M/H]** AU-1: Policy and procedures
- [ ] **[L/M/H]** AU-2: Event logging
- [ ] **[L/M/H]** AU-3: Content of audit records
- [ ] **[M/H]** AU-3(1): Additional audit information
- [ ] **[L/M/H]** AU-4: Audit log storage capacity
- [ ] **[L/M/H]** AU-5: Response to audit processing failures
- [ ] **[L/M/H]** AU-6: Audit review, analysis, and reporting
- [ ] **[M/H]** AU-6(1): Automated audit review
- [ ] **[M/H]** AU-6(3): Correlate audit records
- [ ] **[M/H]** AU-7: Audit reduction and report generation
- [ ] **[L/M/H]** AU-8: Time stamps
- [ ] **[L/M/H]** AU-9: Protection of audit information
- [ ] **[M/H]** AU-11: Audit record retention
- [ ] **[L/M/H]** AU-12: Audit record generation

### Security Assessment and Authorization (CA)
- [ ] **[L/M/H]** CA-1: Policy and procedures
- [ ] **[L/M/H]** CA-2: Control assessments
- [ ] **[M/H]** CA-2(1): Independent assessors
- [ ] **[L/M/H]** CA-3: Information exchange
- [ ] **[L/M/H]** CA-5: Plan of action and milestones
- [ ] **[L/M/H]** CA-6: Authorization
- [ ] **[L/M/H]** CA-7: Continuous monitoring
- [ ] **[L/M/H]** CA-9: Internal system connections

### Configuration Management (CM)
- [ ] **[L/M/H]** CM-1: Policy and procedures
- [ ] **[L/M/H]** CM-2: Baseline configuration
- [ ] **[M/H]** CM-2(1-7): Baseline enhancements
- [ ] **[M/H]** CM-3: Configuration change control
- [ ] **[L/M/H]** CM-4: Impact analyses
- [ ] **[M/H]** CM-5: Access restrictions for change
- [ ] **[L/M/H]** CM-6: Configuration settings
- [ ] **[M/H]** CM-7: Least functionality
- [ ] **[M/H]** CM-7(1-5): Least functionality enhancements
- [ ] **[L/M/H]** CM-8: System component inventory
- [ ] **[M/H]** CM-8(1-5): Inventory enhancements
- [ ] **[M/H]** CM-9: Configuration management plan
- [ ] **[L/M/H]** CM-10: Software usage restrictions
- [ ] **[L/M/H]** CM-11: User-installed software

### Contingency Planning (CP)
- [ ] **[L/M/H]** CP-1: Policy and procedures
- [ ] **[L/M/H]** CP-2: Contingency plan
- [ ] **[M/H]** CP-2(1-8): Contingency plan enhancements
- [ ] **[L/M/H]** CP-3: Contingency training
- [ ] **[L/M/H]** CP-4: Contingency plan testing
- [ ] **[M/H]** CP-6: Alternate storage site
- [ ] **[M/H]** CP-7: Alternate processing site
- [ ] **[L/M/H]** CP-9: System backup
- [ ] **[L/M/H]** CP-10: System recovery and reconstitution

### Identification and Authentication (IA)
- [ ] **[L/M/H]** IA-1: Policy and procedures
- [ ] **[L/M/H]** IA-2: Identification and authentication (organizational users)
- [ ] **[L/M/H]** IA-2(1): MFA for privileged accounts
- [ ] **[M/H]** IA-2(2): MFA for non-privileged accounts
- [ ] **[M/H]** IA-2(8): Replay-resistant authentication
- [ ] **[L/M/H]** IA-4: Identifier management
- [ ] **[L/M/H]** IA-5: Authenticator management
- [ ] **[L/M/H]** IA-5(1): Password-based authentication
- [ ] **[M/H]** IA-5(2): PKI-based authentication
- [ ] **[L/M/H]** IA-6: Authenticator feedback
- [ ] **[L/M/H]** IA-7: Cryptographic module authentication
- [ ] **[L/M/H]** IA-8: Non-organizational user identification/authentication

### Incident Response (IR)
- [ ] **[L/M/H]** IR-1: Policy and procedures
- [ ] **[L/M/H]** IR-2: Incident response training
- [ ] **[L/M/H]** IR-3: Incident response testing
- [ ] **[L/M/H]** IR-4: Incident handling
- [ ] **[M/H]** IR-4(1): Automated incident handling
- [ ] **[L/M/H]** IR-5: Incident monitoring
- [ ] **[L/M/H]** IR-6: Incident reporting
- [ ] **[L/M/H]** IR-7: Incident response assistance
- [ ] **[L/M/H]** IR-8: Incident response plan

### Maintenance (MA)
- [ ] **[L/M/H]** MA-1: Policy and procedures
- [ ] **[L/M/H]** MA-2: Controlled maintenance
- [ ] **[M/H]** MA-3: Maintenance tools
- [ ] **[L/M/H]** MA-4: Nonlocal maintenance
- [ ] **[L/M/H]** MA-5: Maintenance personnel

### Media Protection (MP)
- [ ] **[L/M/H]** MP-1: Policy and procedures
- [ ] **[L/M/H]** MP-2: Media access
- [ ] **[M/H]** MP-3: Media marking
- [ ] **[M/H]** MP-4: Media storage
- [ ] **[M/H]** MP-5: Media transport
- [ ] **[L/M/H]** MP-6: Media sanitization
- [ ] **[L/M/H]** MP-7: Media use

### Physical and Environmental Protection (PE)
- [ ] **[L/M/H]** PE-1: Policy and procedures
- [ ] **[L/M/H]** PE-2: Physical access authorizations
- [ ] **[L/M/H]** PE-3: Physical access control
- [ ] **[L/M/H]** PE-6: Monitoring physical access
- [ ] **[L/M/H]** PE-8: Visitor access records
- [ ] **[M/H]** PE-9: Power equipment and cabling
- [ ] **[M/H]** PE-10: Emergency shutoff
- [ ] **[M/H]** PE-11: Emergency power
- [ ] **[L/M/H]** PE-12: Emergency lighting
- [ ] **[L/M/H]** PE-13: Fire protection
- [ ] **[L/M/H]** PE-14: Temperature and humidity controls
- [ ] **[L/M/H]** PE-15: Water damage protection
- [ ] **[L/M/H]** PE-16: Delivery and removal

### Planning (PL)
- [ ] **[L/M/H]** PL-1: Policy and procedures
- [ ] **[L/M/H]** PL-2: System security and privacy plans
- [ ] **[L/M/H]** PL-4: Rules of behavior
- [ ] **[M/H]** PL-8: Security and privacy architectures

### Personnel Security (PS)
- [ ] **[L/M/H]** PS-1: Policy and procedures
- [ ] **[L/M/H]** PS-2: Position risk designation
- [ ] **[L/M/H]** PS-3: Personnel screening
- [ ] **[L/M/H]** PS-4: Personnel termination
- [ ] **[L/M/H]** PS-5: Personnel transfer
- [ ] **[L/M/H]** PS-6: Access agreements
- [ ] **[L/M/H]** PS-7: External personnel security
- [ ] **[L/M/H]** PS-8: Personnel sanctions

### Risk Assessment (RA)
- [ ] **[L/M/H]** RA-1: Policy and procedures
- [ ] **[L/M/H]** RA-2: Security categorization
- [ ] **[L/M/H]** RA-3: Risk assessment
- [ ] **[L/M/H]** RA-5: Vulnerability monitoring and scanning
- [ ] **[M/H]** RA-5(1-8): Vulnerability scanning enhancements

### System and Services Acquisition (SA)
- [ ] **[L/M/H]** SA-1: Policy and procedures
- [ ] **[L/M/H]** SA-2: Resource allocation
- [ ] **[L/M/H]** SA-3: System development life cycle
- [ ] **[M/H]** SA-4: Acquisition process (security requirements in contracts)
- [ ] **[L/M/H]** SA-5: System documentation
- [ ] **[M/H]** SA-8: Security and privacy engineering principles
- [ ] **[L/M/H]** SA-9: External system services
- [ ] **[M/H]** SA-10: Developer configuration management
- [ ] **[M/H]** SA-11: Developer testing and evaluation

### System and Communications Protection (SC)
- [ ] **[L/M/H]** SC-1: Policy and procedures
- [ ] **[M/H]** SC-2: Separation of system and user functionality
- [ ] **[L/M/H]** SC-5: Denial-of-service protection
- [ ] **[L/M/H]** SC-7: Boundary protection
- [ ] **[M/H]** SC-7(3-13): Boundary protection enhancements
- [ ] **[M/H]** SC-8: Transmission confidentiality and integrity
- [ ] **[M/H]** SC-10: Network disconnect
- [ ] **[M/H]** SC-12: Cryptographic key establishment and management
- [ ] **[L/M/H]** SC-13: Cryptographic protection (FIPS 140-2)
- [ ] **[L/M/H]** SC-15: Collaborative computing devices and applications
- [ ] **[L/M/H]** SC-20: Secure name/address resolution (authoritative source)
- [ ] **[L/M/H]** SC-21: Secure name/address resolution (recursive/caching)
- [ ] **[L/M/H]** SC-22: Architecture and provisioning for name/address resolution
- [ ] **[M/H]** SC-23: Session authenticity
- [ ] **[M/H]** SC-28: Protection of information at rest

### System and Information Integrity (SI)
- [ ] **[L/M/H]** SI-1: Policy and procedures
- [ ] **[L/M/H]** SI-2: Flaw remediation
- [ ] **[M/H]** SI-2(2): Automated flaw remediation status
- [ ] **[L/M/H]** SI-3: Malicious code protection
- [ ] **[L/M/H]** SI-4: System monitoring
- [ ] **[M/H]** SI-4(1-5): System monitoring enhancements
- [ ] **[L/M/H]** SI-5: Security alerts, advisories, and directives
- [ ] **[M/H]** SI-7: Software, firmware, and information integrity
- [ ] **[M/H]** SI-8: Spam protection
- [ ] **[M/H]** SI-10: Information input validation
- [ ] **[M/H]** SI-11: Error handling
- [ ] **[L/M/H]** SI-12: Information management and retention
- [ ] **[M/H]** SI-16: Memory protection

### Supply Chain Risk Management (SR) [H]
- [ ] **[H]** SR-1: Policy and procedures
- [ ] **[H]** SR-2: Supply chain risk management plan
- [ ] **[H]** SR-3: Supply chain controls and processes
- [ ] **[H]** SR-5: Acquisition strategies, tools, and methods
- [ ] **[H]** SR-6: Supplier assessments and reviews
- [ ] **[H]** SR-8: Notification agreements
- [ ] **[H]** SR-11: Component authenticity

## 4. CISA Compliance Requirements

- [ ] Register with CISA for cybersecurity services and threat intelligence
- [ ] Implement CISA Binding Operational Directives within prescribed timeframes
- [ ] Implement CISA Emergency Directives immediately upon issuance
- [ ] Report incidents to CISA/US-CERT per FISMA reporting timelines:
  - [ ] CAT 1 (unauthorized access): Report within 1 hour
  - [ ] CAT 2 (denial of service): Report within 2 hours
  - [ ] CAT 3 (malicious code): Report within 1 hour
  - [ ] CAT 4 (improper usage): Report within 1 week
  - [ ] CAT 5 (scans/probes): Report monthly
  - [ ] CAT 6 (investigation): Report within 1 hour
- [ ] Participate in CDM program (federal agencies) or implement equivalent monitoring
- [ ] Remediate Known Exploited Vulnerabilities (KEV) per BOD 22-01 timelines
- [ ] Deploy endpoint detection and response (EDR) per BOD 22-01

## 5. Inspector General Preparation

- [ ] Maintain current documentation for all systems (SSP, SAR, POA&M)
- [ ] Ensure evidence is organized and readily accessible for each control
- [ ] Prepare maturity level self-assessment across all IG evaluation domains
- [ ] Document corrective actions taken for previous IG findings
- [ ] Prepare briefing materials for IG evaluation team
- [ ] Identify system owners and control implementers for interviews
- [ ] Ensure all personnel have completed required security training
- [ ] Verify all systems have current, valid ATOs
- [ ] Confirm POA&M items are being tracked and remediated on schedule
- [ ] Prepare continuous monitoring reports and dashboards for review

## 6. Zero Trust Architecture Requirements

Per OMB M-22-09 and evolving FISMA guidance:

- [ ] Develop zero trust architecture implementation plan
- [ ] Implement phishing-resistant MFA for all users
- [ ] Deploy device health verification before granting access
- [ ] Implement micro-segmentation for network architecture
- [ ] Encrypt all DNS traffic (DNS over HTTPS/TLS)
- [ ] Encrypt all HTTP traffic (HTTPS everywhere, including internal)
- [ ] Implement continuous authorization and validation
- [ ] Deploy SASE or equivalent cloud security architecture
- [ ] Implement software-defined perimeter concepts
- [ ] Document zero trust maturity progress for FISMA reporting

---

## Resources

- [FISMA (44 U.S.C. 3551-3558)](https://www.govinfo.gov/app/details/USCODE-2018-title44/USCODE-2018-title44-chap35-subchapII)
- [NIST SP 800-53 Rev. 5](https://csrc.nist.gov/publications/detail/sp/800-53/rev-5/final)
- [NIST SP 800-37 Rev. 2 (RMF)](https://csrc.nist.gov/publications/detail/sp/800-37/rev-2/final)
- [NIST SP 800-53A Rev. 5 (Assessment Procedures)](https://csrc.nist.gov/publications/detail/sp/800-53a/rev-5/final)
- [NIST SP 800-53B (Control Baselines)](https://csrc.nist.gov/publications/detail/sp/800-53b/final)
- [NIST SP 800-137 (Continuous Monitoring)](https://csrc.nist.gov/publications/detail/sp/800-137/final)
- [CISA Federal Cybersecurity](https://www.cisa.gov/topics/cybersecurity-best-practices/federal-cybersecurity)
- [PTG FISMA Compliance Services](https://www.petronellatech.com/compliance/fisma/)
- [PTG Compliance Packages](https://www.petronellatech.com/compliance/packages/)

**Need help with FISMA compliance?** Call Petronella Technology Group at 919-348-4912 or visit [https://www.petronellatech.com/compliance/packages/](https://www.petronellatech.com/compliance/packages/) to schedule a free compliance assessment.
