# Controls and Compliance Checklist - Botium Toys Internal Audit

**Auditor:** Adedeji David Adegboyega
**Date:** 2026-11-02
**Framework:** NIST Cybersecurity Framework (CSF) - Identify, Protect, Detect, Respond, Recover

---

## Part 1: Controls Assessment Checklist

Select “yes” or “no” to answer: Does Botium Toys currently have this control in place?

| Control | Yes | No | Explanation |
|---|---|---|---|
| Least Privilege | | X | Currently all employees have access to customer data; privileges need to be limited to reduce breach risk. |
| Disaster recovery plans | | X | No disaster recovery plans in place. Needs implementation to ensure business continuity. |
| Password policies | | X | Employee password requirements are minimal, could allow threat actor to access secure data via employee equipment/internal network. |
| Separation of duties | | X | Needs implementation to reduce fraud risk - CEO currently runs day-to-day operations and manages payroll. |
| Firewall | X | | Existing firewall blocks traffic based on appropriately defined set of security rules. |
| Intrusion detection system (IDS) | | X | IT department needs IDS to identify possible intrusions. |
| Backups | | X | IT department needs backups of critical data to ensure business continuity after breach. |
| Antivirus software | X | | Antivirus software installed and monitored regularly by IT. |
| Manual monitoring, maintenance, and intervention for legacy systems | | X | Legacy systems are monitored/maintained but no regular schedule and intervention policies unclear - at risk of breach. |
| Encryption | | X | Encryption not currently used; implementing would provide greater confidentiality of sensitive information. |
| Password management system | | X | No password management system currently in place; implementing would improve IT productivity for password issues. |
| Locks (offices, storefront, warehouse) | X | | Store's physical location including main offices, store front, and warehouse has sufficient locks. |
| Closed-circuit television (CCTV) surveillance | X | | CCTV installed/functioning at store's physical location. |
| Fire detection/prevention (fire alarm, sprinkler system) | X | | Physical location has functioning fire detection and prevention system. |

**Summary:** 5/14 controls in place, 9 failing.

---

## Part 2: Compliance Checklist

### A. Payment Card Industry Data Security Standard (PCI DSS)

| Best Practice | Yes | No | Explanation |
|---|---|---|---|
| Only authorized users have access to customers' credit card information | | X | Currently all employees have access to company's internal data including credit card data. |
| Credit card information is stored, accepted, processed, transmitted internally in a secure environment | | X | Credit card info not encrypted and all employees have access. |
| Implement data encryption procedures to better secure credit card transaction touchpoints and data | | X | Company does not currently use encryption to ensure confidentiality of customers' financial information. |
| Adopt secure password management policies | | X | Password policies nominal and no password management system in place. |

**Compliance Status:** Non-compliant - High risk of fines and loss of payment processing capability.

### B. General Data Protection Regulation (GDPR)

| Best Practice | Yes | No | Explanation |
|---|---|---|---|
| E.U. customers' data is kept private/secured | | X | Company does not currently use encryption to ensure confidentiality. |
| There is a plan in place to notify E.U. customers within 72 hours if data compromised/breach | X | | Plan to notify within 72 hours exists. |
| Ensure data is properly classified and inventoried | | X | Current assets inventoried/listed but not classified. |
| Enforce privacy policies, procedures, processes to properly document and maintain data | X | | Privacy policies, procedures, processes developed and enforced among IT team and other employees as needed. |

**Compliance Status:** Partially compliant - 2/4. Risk of GDPR fines up to €20M.

### C. System and Organizations Controls (SOC Type 1, SOC Type 2)

| Best Practice | Yes | No | Explanation |
|---|---|---|---|
| User access policies are established | | X | Controls of Least Privilege and separation of duties not in place; all employees have access to internally stored data. |
| Sensitive data (PII/SPII) is confidential/private | | X | Encryption not currently used to ensure confidentiality of PII/SPII. |
| Data integrity ensures data is consistent, complete, accurate, validated | X | | Data integrity in place. |
| Data is available to individuals authorized to access it | | X | While data is available to all employees, authorization needs to be limited to only individuals who need access to do their jobs. |

**Compliance Status:** Partially compliant - 1/4 controls effective.

---

## Part 3: Recommendations

**Priority 1 - Critical (0-30 days):**
1. Implement Least Privilege - RBAC, remove excessive permissions, audit accounting/SIEM/firewall access
2. Implement Separation of Duties - Reassign payroll from CEO to finance/HR with approval workflow
3. Enable Encryption - TLS 1.2+ for online transactions, AES-256 for stored PII/PCI data
4. Deploy Password Manager + MFA + Strong Policy (12+ chars, complexity, lockout)

**Priority 2 - High (30-90 days):**
5. Disaster Recovery & Business Continuity Plan + 3-2-1 backups, test quarterly
6. Deploy IDS/IPS and tune SIEM rules for legacy systems
7. Formal legacy system maintenance schedule with documentation

**Priority 3 - Compliance:**
8. Complete data classification (Public, Confidential, Restricted, PCI, GDPR)
9. Map data flows for E.U. customers, document processing activities (ROPA) for GDPR
10. Conduct quarterly access reviews and annual SOC readiness assessment
