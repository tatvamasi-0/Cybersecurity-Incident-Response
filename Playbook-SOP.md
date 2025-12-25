BankX – TechA Joint Incident Response Playbook
**Document Type:** Standard Operating Procedures (SOP)  
**Purpose:** To define coordinated technical and strategic actions when a data breach impacts BankX’s customer data through TechA’s infrastructure.  
**Scope:** Applies to all phases of incident response, escalation, and communication activities.


**Phase 1: Identification**

**Objective**
Detect, confirm, and understand the scope of the incident.

** Key Activities**
1. **Query and Analyze Logs**  
   - Use SIEM tools to locate malicious Indicators of Compromise (IoCs).  
   - Correlate endpoints, access tokens, and user accounts showing anomalies.  
   - Identify if internal or third-party systems accessed or exfiltrated data.

2. **Evidence Preservation**  
   - Snapshot affected systems and network traffic logs.
   - Maintain evidence chain for forensic and legal review.

3. **Notification Flow**  
   - TechA Tech Lead → TechA CTO/CIO → BankX CISO → BankX CEO.
   - Document findings in Incident Tracker.

 **Role Responsibilities**

| Role | Organization | Responsibilities in Identification |
|------|---------------|-----------------------------------|
| **CEO** | BankX | Approve official acknowledgment, initiate executive awareness briefing. |
| **CEO** | TechA | Authorize use of technical and legal resources for investigation. |
| **CIO** | TechA | Coordinate technical response team, oversee data collection and investigations. |
| **CTO** | TechA | Validate IoCs, audit system vulnerabilities, and assist forensic validation. |
| **Tech Lead** | TechA | Execute log analysis, confirm breach vectors, and prepare containment recommendations. |
| **Employee Y** | TechA | Refrain from unauthorized disclosure; cooperate with investigation (incident witness). |
| **CISO** | BankX | Receive initial findings, assess compliance implications, liaise with regulators if required. |
| **Security Analyst** | BankX | Validate IoCs from TechA and confirm breach boundaries. |
| **CFO** | BankX | Assess potential financial exposure and allocate emergency response budget. |
| **PR Head** | BankX | Remain on standby for incident communication after official containment. |



** Phase 2: Containment**

** Objective**
Prevent further compromise or data exfiltration while maintaining service continuity.

 **Key Activities**
1. **Access and Token Control**
   - Revoke active **refresh tokens** tied to compromised accounts.
   - Apply strict **Conditional Access** rules (e.g., MFA enforcement, geo restrictions).

2. **Network Control**
   - Quarantine affected systems from production.
   - Disable access accounts and rotate keys associated with affected APIs/services.

3. **Communication Control**
   - All internal and external communications must follow the established chain of command.

 **Role Responsibilities**

| Role | Organization | Responsibilities in Containment |
|------|---------------|--------------------------------|
| **CEO** | BankX | Approve public posture after regulator and PR consultation. |
| **CEO** | TechA | Authorize temporary service restrictions impacting availability. |
| **CIO** | TechA | Oversee all containment steps and change-control approvals. |
| **CTO** | TechA | Direct engineers to execute revocations and token resets. |
| **Tech Lead** | TechA | Implement containment scripts and validate Conditional Access enforcement. |
| **CISO** | BankX | Approve containment strategy and ensure customer data safeguards meet regulatory expectations. |
| **Security Analyst** | BankX | Verify isolation effectiveness and lack of residual exposure. |
| **CFO** | BankX | Track response-related expenses and potential penalties. |
| **PR Head** | BankX | Draft internal/external statements based on executive review. |
| **Employee Y** | TechA | Cooperate fully with HR and compliance; restricted from communications pending review. |



**Phase 3: Eradication**

**Objective**
Remove all persistence mechanisms, malicious code, and restore secure operations.

**Key Activities**
1. **Identify and Remove Backdoor**
   - Audit **App Registrations** and linked credentials.
   - Remove unauthorized “backdoor” registrations or API connections.

2. **Credential and Configuration Reset**
   - Regenerate API keys and revalidate OAuth information sharing between BankX and TechA systems.

3. **Verification & Closure**
   - Conduct full vulnerability scan.
   - BankX Security Analyst cross-checks system health.

** Role Responsibilities**

| Role | Organization | Responsibilities in Eradication |
|------|---------------|--------------------------------|
| **CEO (Both)** | BankX & TechA | Jointly approve post-eradication report and public disclosure decisions. |
| **CIO** | TechA | Confirm eradication success and authorize system restoration. |
| **CTO** | TechA | Oversee patch management and verify reauthorization procedures. |
| **Tech Lead** | TechA | Execute technical fixes and document eradication evidence. |
| **CISO** | BankX | Validate compliance steps, ensure data confidentiality restored. |
| **Security Analyst** | BankX | Review remediation logs and conduct post-action testing. |
| **CFO** | BankX | Quantify incident financial closure and insurance claim coordination. |
| **PR Head** | BankX | Roll out final public statement under legal oversight. |
| **Employee Y** | TechA | Subject to internal HR and compliance inquiry per disclosure violation. |



## Post-Eradication Activities
- Conduct **joint review session** with all roles.  
- Prepare for **Regulatory and Audit Reporting** within 72 hours.  
- Initiate **Post-Mortem Analysis** using the template below.  
