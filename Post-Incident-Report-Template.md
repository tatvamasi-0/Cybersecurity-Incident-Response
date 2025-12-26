# Post-Incident Report Template  
**BankX / TechA Joint Follow-Up Review**



** 1. Summary
**
- **Incident Name/ID:** [Identifier Code]  
- **Incident Type:** PII Breach via Vendor System  
- **Date Detected:** [Insert Date]  
- **Initial Reporter:** TechA Tech Lead  
- **Impact Scope:** 5,000 BankX Customers  



** 2. Timeline of Events
**
| Time | Event | Stakeholder | Notes |
| [T1] | Initial anomaly detected in TechA logs | Tech Lead | Unusual token usage pattern |
| [T2] | Notification sent to BankX CISO | CIO – TechA | Incident escalated |
| [T3] | Containment actions began | CTO – TechA | Tokens revoked, CA rules updated |
| [T4] | Internal review completed | CISO – BankX | Data exposure validated |
| [T5] | Public leak by employee | HR/PR – TechA | Press involvement initiated |
| [T6] | Eradication verified and closed | Both CIOs | Backdoor app removed |
| [T7] | Joint lessons learned meeting | All Parties | Playbook finalization |



** 3. Root Cause Analysis (RCA)**
- **Primary Cause:** Unauthorized app registration enabling external access to PII storage APIs.  
- **Secondary Cause:** Ineffective conditional access monitoring at TechA.  
- **Tertiary Component:** Insider mishandling of confidential information, leading to public disclosure.



** 4. Impact Assessment**
| Impact Area | Severity | Description |
| Customer Data Exposure | High | 5,000 PII records |
| Operational Downtime | Low | 2–4 hours service disruption |
| Compliance/Regulatory | Medium | SOX/NERC CIP review pending |
| Reputational Risk | High | Public media coverage |


** 5. Gap Analysis **
| Category | Identified Gap | Recommendation |
| Detection | Insufficient IoC correlation alerts in TechA SIEM | Deploy ML-driven anomaly detection |
| Containment | Token revocation not automated | Integrate automated incident API workflows |
| Governance | Employee NDA enforcement weak | Reinforce disclosure clause and training |
| Communication | Delayed legal notification | Standardize 24-hour compliance escalation SLA |



** 6. Lessons Learned
**
- Early joint-monitoring could have reduced detection latency.  
- Containment workflows need automated API-based revocations.  
- Insider awareness policies must include breach confidentiality protocols.  

---

** 7. Action Plan
**
| Task | Responsible Role | Deadline |
| Implement enhanced conditional access monitoring | Tech Lead – TechA | [Date] |
| Conduct co-sponsored tabletop exercise | CISO – BankX | [Date] |
| Reinforce NDA and data handling training | HR – TechA | [Date] |
| Establish regulator communication SLA | Legal – BankX | [Date] |
