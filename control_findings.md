# FedRAMP / NIST SP 800-53 Control Findings

## Purpose

This document summarizes control weaknesses identified during the simulated FedRAMP-aligned NIST SP 800-53 control assessment for CloudNova Federal Cloud.

The review focuses on access control, audit logging, configuration management, contingency planning, authentication, incident response, vulnerability remediation, and supply-chain risk.

---

## Finding 1: Account Management

### Control

**AC-2 – Account Management**

### Current State

User provisioning and termination processes exist, but recurring account reviews are inconsistent.

### Risk

Inactive or unnecessary accounts may remain enabled and provide unauthorized access to cloud systems.

### Risk Level

**High**

### Gap

The organization does not consistently validate that accounts remain necessary.

### Recommendation

Perform quarterly account reviews and document:

- Account owner
- Business justification
- Account status
- Reviewer decision
- Removed access
- Review date

Automate terminated-user account disabling where possible.

---

## Finding 2: Least Privilege

### Control

**AC-6 – Least Privilege**

### Current State

Role-based access control is implemented, but privileged-access reviews are incomplete.

### Risk

Users may retain elevated permissions that are no longer required.

### Risk Level

**High**

### Gap

Privileged access is not reviewed consistently.

### Recommendation

Perform quarterly privileged-access reviews and document:

- Privileged account
- Assigned role
- Business justification
- Account owner
- Reviewer
- Approval decision
- Removed privileges

Apply least privilege wherever possible.

---

## Finding 3: Audit Record Review

### Control

**AU-6 – Audit Record Review, Analysis, and Reporting**

### Current State

Security logs are centrally collected, but recurring review evidence is incomplete.

### Risk

Suspicious or unauthorized activity may remain undetected.

### Risk Level

**Medium**

### Gap

Audit-log review activity is not consistently documented.

### Recommendation

Define recurring log-review procedures that document:

- Review frequency
- Reviewer
- Systems reviewed
- Suspicious events
- Investigation tickets
- Escalation decisions
- Resolution

---

## Finding 4: Baseline Configuration

### Control

**CM-2 – Baseline Configuration**

### Current State

Secure configuration standards exist, but formal review evidence is incomplete.

### Risk

Outdated baseline configurations may introduce avoidable security weaknesses.

### Risk Level

**Medium**

### Gap

Configuration baselines are not consistently reviewed and approved.

### Recommendation

Review secure configuration baselines annually and after significant technology changes.

Document:

- Baseline owner
- Review date
- Changes
- Approval
- Next review date

---

## Finding 5: Configuration Exceptions

### Control

**CM-6 – Configuration Settings**

### Current State

Secure settings are defined, but exceptions are not centrally tracked.

### Risk

Insecure or unapproved configurations may persist without management visibility.

### Risk Level

**Medium**

### Gap

There is no centralized configuration-exception process.

### Recommendation

Create a configuration exception register including:

- System
- Setting
- Reason for exception
- Risk level
- Compensating control
- Owner
- Due date
- Approval
- Closure status

---

## Finding 6: System Recovery Testing

### Control

**CP-10 – System Recovery and Reconstitution**

### Current State

Regular backups are performed, but restoration testing is inconsistent.

### Risk

Systems may not be recoverable during ransomware, outages, or disaster recovery events.

### Risk Level

**Medium**

### Gap

The organization lacks consistent evidence that critical systems can be restored.

### Recommendation

Perform quarterly restoration tests and document:

- System tested
- Backup selected
- Test date
- Recovery result
- Recovery time
- Issues identified
- Corrective actions

---

## Finding 7: MFA for Privileged Accounts

### Control

**IA-2(1) – Multi-Factor Authentication for Privileged Accounts**

### Current State

MFA is enabled for some privileged accounts but not all.

### Risk

Compromised privileged credentials may provide broad access to critical cloud resources.

### Risk Level

**High**

### Gap

Strong authentication is not consistently enforced for privileged access.

### Recommendation

Require MFA for all privileged accounts.

Document:

- Privileged account inventory
- MFA enrollment
- Approved exceptions
- Exception owner
- Review date

---

## Finding 8: MFA for Remote Access

### Control

**IA-2(2) – Multi-Factor Authentication for Non-Privileged Accounts**

### Current State

MFA is used for remote access, but coverage is not consistently validated.

### Risk

Some users may access cloud resources without strong authentication.

### Risk Level

**Medium**

### Gap

MFA enrollment and coverage are not fully verified.

### Recommendation

Perform recurring MFA coverage reviews and confirm that all applicable remote users are enrolled.

---

## Finding 9: Incident Response Testing

### Control

**IR-3 – Incident Response Testing**

### Current State

Incident response procedures exist, but tabletop exercises are not performed consistently.

### Risk

Teams may respond slowly or inconsistently during a real security incident.

### Risk Level

**High**

### Gap

Incident response procedures are not regularly validated.

### Recommendation

Conduct annual tabletop exercises and document:

- Scenario
- Participants
- Response actions
- Escalation decisions
- Communication process
- Lessons learned
- Corrective actions

---

## Finding 10: Flaw Remediation

### Control

**SI-2 – Flaw Remediation**

### Current State

Vulnerability findings are tracked, but some high-risk items exceed target remediation timelines.

### Risk

Known vulnerabilities may remain exploitable longer than acceptable.

### Risk Level

**High**

### Gap

Severity-based remediation timelines are not consistently enforced.

### Recommendation

Establish remediation targets such as:

- Critical: 7 Days
- High: 30 Days
- Medium: 60 Days
- Low: 90 Days

Approved exceptions should require documented risk acceptance.

---

## Finding 11: Supply Chain Risk Management

### Control

**SR-3 – Supply Chain Controls and Processes**

### Current State

Vendor security assessments occur, but recurring reassessment is inconsistent.

### Risk

High-risk suppliers may introduce unmanaged cybersecurity risk.

### Risk Level

**High**

### Gap

High-risk suppliers are not consistently reassessed.

### Recommendation

Perform annual reassessments covering:

- Vendor risk classification
- Security questionnaire
- Compliance evidence
- Data access
- Incident notification
- Subcontractors
- Open findings
- Remediation status

---

## Finding 12: Risk Assessment Evidence

### Control

**RA-3 – Risk Assessment**

### Current State

Risk assessments are performed, but supporting evidence is spread across multiple locations.

### Risk

Audit readiness may be reduced because required documentation is difficult to retrieve.

### Risk Level

**Medium**

### Gap

Risk-assessment evidence is not centrally organized.

### Recommendation

Create a centralized evidence repository containing:

- Risk assessments
- Risk registers
- Management reviews
- Risk approvals
- Remediation records
- Supporting evidence

---

## Overall Findings Summary

| Finding | Control | Risk Level |
|---|---|---|
| Account Management | AC-2 | High |
| Least Privilege | AC-6 | High |
| Audit Record Review | AU-6 | Medium |
| Baseline Configuration | CM-2 | Medium |
| Configuration Exceptions | CM-6 | Medium |
| System Recovery Testing | CP-10 | Medium |
| MFA for Privileged Accounts | IA-2(1) | High |
| MFA for Remote Access | IA-2(2) | Medium |
| Incident Response Testing | IR-3 | High |
| Flaw Remediation | SI-2 | High |
| Supply Chain Risk Management | SR-3 | High |
| Risk Assessment Evidence | RA-3 | Medium |

---

## Conclusion

The assessment identified several high-priority weaknesses involving account management, privileged access, MFA, vulnerability remediation, incident response, and supply-chain risk.

Medium-risk findings involve audit-log review, configuration management, system recovery testing, and evidence organization.

These findings should be tracked through the POA&M until remediation is completed and validated.
