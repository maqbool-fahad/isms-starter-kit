# Access Control Policy: Havelmetrics GmbH

## 1. Purpose

This policy makes sure people have the access they need to do their job and nothing more. It supports the Information Security Policy (see information-security-policy.md) and the customer contracts that depend on ISO 27001.

## 2. Scope

All employees, contractors and suppliers, and these systems: Microsoft 365 and Entra ID, Azure (including Azure SQL), GitHub, the customer support tool, company laptops, and personal phones used for work email (see isms-scope.md).

## 3. Rules

**Accounts and sign-in**
- Every person has one unique Entra ID account. Shared accounts are not allowed.
- Multi-factor authentication (MFA) is required for all staff accounts by 18 November 2026 (risk R01). Administrators use passkeys or hardware security keys (risk R02).
- Passwords are kept in the company password manager and are never reused (risk R17).
- Biometric unlock is used only on the person's own device. Havelmetrics never collects or stores biometric data.
- GitHub is accessed through single sign-on with Entra ID, with MFA for every member (risk R12).

**Administrator access**
- Administrators do admin work only with a separate admin account, never their daily account.
- Two emergency (break-glass) accounts are held by two different trusted people, so administration does not depend on the part-time IT Administrator alone (risk R10).
- Production changes are reviewed by a second person before release.

**Joiners, movers and leavers**
- Access is given by role. Extra access needs approval from the system owner.
- When someone changes role, their access is reviewed within five working days.
- Leavers lose all access on their last working day. A checklist covers Microsoft 365 and Entra ID, Azure, GitHub, the support tool, the password manager, equipment and work email on personal phones. It is in use by 17 January 2027 (risks R07 and R13).

**Reviews**
- Access to Azure, the database, GitHub, the support tool and administrator roles is reviewed every quarter by the system owner. All other access is reviewed once a year. Each review is recorded.

**Customer data and secrets**
- The customer database is reachable through private endpoints only, with access by named roles (risk R03). Support staff see only what a ticket needs (risk R26).
- Real customer data is never copied into the test environment (risk R15).
- Passwords, keys and certificates are never stored in code. They live in Azure Key Vault. GitHub secret scanning is on, and any exposed secret is replaced at once (risks R11 and R27).

## 4. Roles

- **Management** approves this policy.
- **ISMS Manager** maintains it and reports on reviews and exceptions.
- **IT Administrator** creates, changes and removes access.
- **System owners** (Head of Engineering for Azure and GitHub, Head of Sales and Support for the support tool) approve access and run the reviews.
- **Head of Operations** owns the leaver process.
- **All staff** protect their accounts and report anything suspicious (see incident-response-policy.md).

## 5. Exceptions

Exceptions must be requested in writing, approved by the ISMS Manager, limited in time and recorded. Significant exceptions are added to the risk register.

## 6. Traceability

- **Controls (see statement-of-applicability.xlsx):** 5.3, 5.15, 5.16, 5.17, 5.18, 6.5, 8.2, 8.3, 8.5
- **Risks (see risk-register.xlsx):** R01, R02, R03, R07, R10, R11, R12, R13, R15, R17, R26, R27

## 7. Review and approval

Reviewed once a year and after any major incident or change. Next review: October 2027.

Approved by: Jonas Becker, Chief Executive Officer
Date: 24 October 2026
Version: 1.0
