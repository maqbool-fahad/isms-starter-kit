# Incident Response Policy: Havelmetrics GmbH

## 1. Purpose

This policy sets out how Havelmetrics reports, handles and learns from security incidents, and how it meets legal and contractual deadlines, including the 72-hour deadline for personal data breaches under GDPR. It supports the Information Security Policy (see information-security-policy.md).

## 2. Scope

All employees, contractors and suppliers, and all systems in the ISMS scope (see isms-scope.md).

## 3. Roles

- **Incident Coordinator:** the ISMS Manager. Leads the response, keeps the incident log and makes sure deadlines are met.
- **Technical Lead:** the Head of Engineering. Decides and carries out containment and recovery, with the IT Administrator.
- **CEO:** told immediately of every Severity 1 incident. Decides on notifications to authorities and customers.
- **Customer communication:** the Head of Sales and Support, with the CEO.
- **All staff:** report events promptly and follow instructions.

A short on-call arrangement between the ISMS Manager and the Head of Engineering covers evenings and weekends for Severity 1 incidents, because there is only one part-time IT Administrator.

## 4. Reporting

- Anyone who suspects an incident reports it at once, and at the latest within 24 hours of discovery. It is logged within the same 24 hours (risk R19).
- Reports go to the Teams channel #security-incidents or the mailbox security@havelmetrics.example. Severity 1 events are also reported by phone.
- Reporting in good faith is never punished.

## 5. Severity

| Severity | Examples | First response |
|---|---|---|
| 1 Critical | Customer data breach, ransomware, compromised administrator account, long production outage | Within 1 hour, CEO informed |
| 2 High | Suspected data breach, compromised staff account, malware, major supplier breach | Within 4 hours |
| 3 Medium | Lost encrypted laptop, phishing clicked without sign-in | Within 1 working day |
| 4 Low | Spam, blocked attacks, policy breaches without data impact | Within 3 working days |

## 6. Handling

1. **Report and log** the event.
2. **Assess** it and set the severity. Decide whether personal data is affected.
3. **Contain** it: disable affected accounts, isolate devices, revoke keys. Do not wipe systems before evidence is saved, unless needed to stop serious harm.
4. **Keep evidence:** logs, screenshots, device images. Keep them for the investigation and at least 12 months afterwards.
5. **Recover:** remove the cause, restore from clean backups, change credentials, and keep security controls in place.
6. **Notify** where required (section 7).
7. **Review** within 10 working days for Severity 1 and 2: what happened, what worked, what changes. Update the risk register and policies.

## 7. Notification

- **Personal data breach, Havelmetrics as controller** (for example its own staff data): if there is a risk to people, notify the Berlin data protection authority within 72 hours of becoming aware. If the risk is high, inform the people affected without undue delay.
- **Personal data breach, Havelmetrics as processor** (customers' data in StoreSight): tell the customer without undue delay and within the time in the contract. The customer decides on notifying the authority.
- **NIS2:** applicability is still being assessed (risk R24). If it applies, the process must support an early warning within 24 hours, a notification within 72 hours and a final report within one month.
- Every decision on whether to notify, including a decision not to, is recorded with the reasons (see Appendix).
- Only the CEO or a named person speaks to customers, authorities or the press.

## 8. Practice and records

- A tabletop exercise is held at least once a year, the first by 17 January 2027 (risk R23).
- The incident log records: date and time, reporter, description, systems and data affected, severity, actions, notifications, cause and lessons learned.

## 9. Traceability

- **Controls (see statement-of-applicability.xlsx):** 5.24, 5.25, 5.26, 5.27, 5.28, 5.29, 6.8
- **Risks (see risk-register.xlsx):** R19, R23, R24. Also supports the response to R01, R02, R14 and R30.

## 10. Review and approval

Reviewed once a year and after any major incident or change. Next review: October 2027.

Approved by: Jonas Becker, Chief Executive Officer
Date: 24 October 2026
Version: 1.0

---

## Appendix: personal data breach checklist (72 hours)

1. When did Havelmetrics become aware? (This starts the 72-hour clock.)
2. What personal data is affected, and about how many people?
3. Is it Havelmetrics's own staff data, or a customer's data in StoreSight?
4. Was the data encrypted or unreadable to whoever accessed it?
5. Could it harm the people affected? Is the risk unlikely, a risk, or high? Write the reason.
6. If processor: which customers are affected, and by when must each be told?
7. If controller and there is a risk: notify the authority within 72 hours. If details are missing, send what is known and add the rest later.
8. If the risk is high: inform the people affected.
9. Who decided, when, and why? Record it, including a decision not to notify.
