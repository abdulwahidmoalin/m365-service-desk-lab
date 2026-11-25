# Microsoft 365 Service Desk Lab

A hands-on lab simulating real service desk work: incidents, service requests, joiners and leavers. Tickets are logged and tracked in **ServiceNow** and resolved in **Microsoft 365** (Entra ID, Exchange Online, Intune).

Every scenario follows the same flow a real 1st/2nd line analyst would use: take the call, log and prioritise the ticket, verify the user, fix the issue in the admin tools, confirm with the user, then document and resolve.

## Tech used

| Area | Tools |
|---|---|
| Identity and access | Microsoft Entra ID, Microsoft 365 admin center |
| Email and calendars | Exchange Online, Outlook |
| Device management | Microsoft Intune |
| Security | Conditional Access, MFA |
| ITSM | ServiceNow (incident and request management, SLAs, knowledge base) |

## The lab company

**Moalin IT Lab** is a fictional company on a Microsoft 365 Business Premium tenant. Its staff are characters from *The Wire*:

| User | Role | Department |
|---|---|---|
| Cedric Daniels | Operations Manager | Management |
| Lester Freamon | IT Support Engineer | IT |
| Kima Greggs | Operations Analyst | Operations |
| Jimmy McNulty | Operations Analyst | Operations (leaver) |
| Bunk Moreland | Operations Analyst | Operations (new starter) |

Tickets are assigned to the **Moalin Service Desk** group in ServiceNow. Setup details: [00-setup](00-setup/README.md)

## Scenarios

| # | Ticket | Scenario | Skills | Status |
|---|---|---|---|---|
| 01 | INC0010002 | [Forgotten password](scenarios/01-password-reset/README.md) | Entra ID, identity verification, password reset | ✅ Done |
| 02 | INC0010006 | Outlook keeps prompting for password | Microsoft 365, sign-in sessions, Credential Manager | ⏳ Planned |
| 03 | INC0010003 | Email not received | Exchange Online message trace | ⏳ Planned |
| 04 | INC0010004 | Blocked sign-in when working from home | Conditional Access, sign-in logs | ⏳ Planned |
| 05 | INC0010005 | New app not installed on laptop | Intune app assignment, device compliance | ⏳ Planned |
| 06 | REQ0010001 | [Leaver: Jimmy McNulty](scenarios/06-leaver-mcnulty/README.md) | Block sign-in, revoke sessions, shared mailbox, Full Access, licence removal | ✅ Done |
| 07 | REQ0010002 | Calendar delegation | Exchange calendar permissions | ⏳ Planned |
| 08 | REQ0010003 | Shared mailbox access | Full Access and Send As permissions | ⏳ Planned |
| 09 | REQ0010004 | New starter: Bunk Moreland | User creation, licensing, groups, mailbox | ⏳ Planned |

## Reference notes

- [ITSM notes: priority, SLAs, work notes vs comments](docs/itsm-notes.md)
- [Knowledge base articles](knowledge-base/)

## About me

I'm Abdulwahid Moalin, an IT support engineer based in London with a BEng in Information and Communication Technology. I built this lab to practise and demonstrate service desk skills end to end.

[LinkedIn](https://www.linkedin.com/in/abdulwahidmoalin)
