# 🔐 IAM Policy Audit Simulator — TechNova Inc.

> A simulated Identity & Access Management audit for a fictional fintech company, demonstrating core IAM concepts, access control analysis, risk assessment, and professional security reporting.

---

## 📋 Project Overview

This project simulates a real-world IAM audit engagement for **TechNova Inc.**, a fictional 25-person fintech startup. As the auditing IAM Analyst, I reviewed the company's complete user access register across 6 departments and 6 business systems, identified security violations, rated them by risk severity, and produced a professional audit report with a remediation roadmap.

The project was built as part of a cybersecurity and IAM portfolio to demonstrate both technical and strategic competency in identity and access management.

---

## 🏢 About TechNova Inc. (Fictional Company)

| Detail | Value |
|---|---|
| **Industry** | Fintech — Payment Processing Software |
| **Employees Audited** | 25 |
| **Departments** | Engineering, Finance, HR, Management, Marketing, Sales, IT Support |
| **Systems in Scope** | CoreBanking, HR Portal, GitHub Enterprise, AWS Console, Jira, Slack |
| **Audit Date** | June 2025 |
| **Frameworks Referenced** | ISO 27001, SOC 2 Type II, GDPR, PCI-DSS |

> ⚠️ All data, employee names, and company details in this project are entirely fictional and created for portfolio purposes only.

---

## 📁 Repository Structure

```
iam-policy-audit/
│
├── data/
│   └── TechNova_IAM_Audit.xlsx        # User Access Register + Audit Findings
│
├── report/
│   └── TechNova_IAM_Audit_Report.docx # Full professional audit report
│
└── README.md                           # Project documentation (this file)
```

---

## 🔍 What Was Audited

### Access Levels Used
| Level | Description |
|---|---|
| **Admin** | Full control — create, modify, delete |
| **Read/Write** | Can view and edit data |
| **Read Only** | View access only |
| **No Access** | Not provisioned on this system |

### Violation Types Identified
| Violation Type | Description |
|---|---|
| **Orphaned Account** | Active accounts belonging to terminated employees |
| **Privilege Creep** | Users who changed roles but retained prior access |
| **Segregation of Duties Conflict** | Users who can both initiate and approve sensitive actions |
| **Excessive Privilege (PoLP Violation)** | Access beyond what the role requires |
| **Unauthorised Access** | Access with no business justification for the role |
| **Overdue Access Review** | Access not reviewed within the required 12-month window |

---

## 📊 Audit Findings Summary

| Risk Rating | Count | Action Window |
|---|---|---|
| 🔴 **Critical** | 3 | Immediate — within 24–48 hours |
| 🟠 **High** | 6 | Within 7 days |
| 🟡 **Medium** | 3 | Within 30 days |
| 🟢 **Low** | 0 | — |
| **Total** | **12** | |

### Critical Findings at a Glance
| ID | Violation | Employee | Risk |
|---|---|---|---|
| AF-001 | Orphaned Account | TN-011 Kevin Okafor (Terminated) | 🔴 Critical |
| AF-002 | Orphaned Account + AWS Admin Access | TN-022 Yuki Tanaka (Terminated) | 🔴 Critical |
| AF-003 | Segregation of Duties Conflict | TN-021 Rohan Desai (Accounts Payable) | 🔴 Critical |

---

## 🛡️ IAM Concepts Demonstrated

**Principle of Least Privilege (PoLP)**
Every user should only have the minimum access required to perform their job. Violations were found across junior, intern, and IT support roles holding Admin-level access to critical systems.

**Role-Based Access Control (RBAC)**
Access entitlements are assigned based on job role. The audit identified multiple users whose access did not align with their current role, including a Finance Manager who retained Engineering-era entitlements after an internal role change.

**Segregation of Duties (SoD)**
No individual should be able to both initiate and authorise a sensitive action. An Accounts Payable employee was found with Admin-level payment system access, creating a direct financial fraud risk.

**Orphaned Account Management**
All accounts must be disabled upon termination. Two terminated employees had fully active accounts — one with live AWS Admin access over 12 months after leaving the company.

**Privilege Creep**
When users change roles, prior access must be revoked. One Finance Manager who moved from Engineering was found retaining entitlements from both roles simultaneously.

**Access Review Cadence**
User access must be formally reviewed at least every 12 months. Two users were identified with overdue reviews, representing a compliance gap against ISO 27001 and SOC 2 requirements.

---

## 📄 Key Deliverables

### 1. User Access Register (`data/TechNova_IAM_Audit.xlsx` — Sheet 1)
- Complete entitlement register for all 25 employees
- Colour-coded access matrix (Admin = red, Read/Write = amber, Read Only = green)
- Terminated employee rows highlighted for immediate visibility
- Access levels mapped across all 6 business systems

### 2. Audit Findings Sheet (`data/TechNova_IAM_Audit.xlsx` — Sheet 2)
- 12 formally documented findings (AF-001 to AF-012)
- Each finding includes: violation type, systems affected, description, risk rating, recommended action, remediation priority, and status
- Summary block showing Critical / High / Medium breakdown

### 3. Audit Report (`report/TechNova_IAM_Audit_Report.docx`)
- **Section 1:** Executive Summary with findings scoreboard and immediate action table
- **Section 2:** Audit scope, methodology, and framework alignment
- **Section 3:** IAM policy framework reference table
- **Section 4:** All 12 detailed findings with colour-coded risk blocks
- **Section 5:** Four-tier remediation roadmap (48hr → 7 days → 30 days → 90 days)
- **Section 6:** Conclusion and management recommendations

---

## 🧰 Tools & Skills Used

| Category | Detail |
|---|---|
| **Spreadsheet** | Microsoft Excel — data modelling, conditional formatting, colour-coded matrices |
| **Documentation** | Microsoft Word — professional report writing, structured findings, executive communication |
| **Frameworks** | ISO 27001, SOC 2 Type II, GDPR, PCI-DSS |
| **IAM Concepts** | PoLP, RBAC, SoD, orphaned account management, privilege creep, access review |
| **Security Domains** | Identity & Access Management, Risk Assessment, Compliance, Audit Reporting |

---

## 🎯 Key Takeaways

- Fintech environments require strict access controls due to the sensitivity of payment data and regulatory obligations
- Orphaned accounts represent one of the most common and highest-risk IAM failures in real organisations
- A Segregation of Duties failure in a Finance system is not just a security issue — it is a financial controls issue that auditors and regulators treat as a serious finding
- Junior and intern roles are frequently over-provisioned during onboarding and rarely reviewed, making them a consistent source of least privilege violations
- Access reviews are a compliance requirement under ISO 27001 and SOC 2 — not just a best practice

---

## 🔗 Part of My Cybersecurity Portfolio

This is **Project 1 (Tier 1)** of my IAM and cybersecurity portfolio. The portfolio is being built to demonstrate both technical and strategic skills in identity security, with projects progressing from foundational IAM analysis through to hands-on technical builds and threat modelling.

| Project | Status |
|---|---|
| Project 1 — IAM Policy Audit Simulator | ✅ Complete |
| Project 2 — Zero Trust Architecture Proposal | 🔜 Coming Soon |
| Project 3 — SSO & MFA Home Lab | 🔜 Coming Soon |
| Project 4 — Access Review Automation Script | 🔜 Coming Soon |
| Project 5 — Threat Modelling Report | 🔜 Coming Soon |
| Project 6 — IAM Security Dashboard | 🔜 Coming Soon |

---

*Disclaimer: All company names, employee names, and data in this project are entirely fictional and created solely for portfolio and educational purposes.*
