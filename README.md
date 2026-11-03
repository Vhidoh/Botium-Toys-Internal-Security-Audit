# Botium Toys - Internal Security Audit
Google Cybersecurity Professional Certificate | Course 2: Manage Security Risks

## Scenario
Botium Toys is a small U.S. business that develops and sells toys. The business has a single physical location, which serves as their main office, a storefront, and warehouse. Online presence has grown globally, increasing pressure on IT. The IT manager initiated an internal IT audit using the National Institute of Standards and Technology Cybersecurity Framework (NIST CSF) to identify risks, threats, vulnerabilities, and ensure compliance with PCI DSS and GDPR.

## Audit Scope & Goals

**Scope:**
- Current user permissions in: accounting, endpoint detection, firewalls, IDS, SIEM tool
- Current implemented controls in: accounting, endpoint detection, firewalls, IDS, SIEM tool

**Goals:**
- Adhere to NIST CSF
- Establish a better process for compliance
- Fortify system controls
- Implement principle of least privilege and separation of duties
- Ensure PCI DSS and GDPR compliance

## Methodology
Reviewed Botium Toys: Scope, goals, and risk assessment report + Controls categories. Completed Controls Assessment and Compliance Checklists aligned to NIST CSF Identify, Protect, Detect, Respond, Recover functions.

## Key Findings
- **Controls:** 8 of 13 controls failing - No Least Privilege, No Disaster Recovery, Weak Password Policies, No Separation of Duties, No IDS, No Backups, No Encryption, No Password Management
- **PCI DSS:** 0/4 compliant - All employees have access to credit card data, no encryption, no secure password management
- **GDPR:** 2/4 compliant - 72-hour breach notification plan exists and privacy policies enforced, but E.U. data not secured/encrypted and data not classified
- **SOC 1 & 2:** 1/4 compliant - Data integrity in place, but access policies not established and PII/SPII not confidential

## Recommendations
1. Implement Least Privilege & Separation of Duties immediately
2. Deploy encryption for PII/SPII and cardholder data (at rest & in transit)
3. Implement enterprise password manager + strong password policy + MFA
4. Create Disaster Recovery Plan and 3-2-1 backup strategy with tested restores
5. Deploy IDS/IPS and centralize monitoring in SIEM
6. Classify data and complete asset inventory per GDPR Article 30
7. Schedule regular maintenance for legacy systems

## Risks & Fines if Not Addressed
- PCI DSS: Fines, loss of ability to process payments, legal liability
- GDPR: Up to €20M or 4% of annual global turnover
- SOC: Loss of customer trust and contracts
- General: Data breach, business disruption, fraud

## Frameworks & Compliance
NIST Cybersecurity Framework (CSF), PCI DSS, GDPR, SOC Type 1 / Type 2

## Files in this Repo
- /docs/Controls-and-Compliance-Checklist.md - Full completed checklist
- /docs/Botium-Toys-Audit-Report.pdf - Formatted PDF report for submission
- /assets/ - Screenshots / evidences

## Author
Adedeji David Adegboyega - Aspiring Cybersecurity Analyst
