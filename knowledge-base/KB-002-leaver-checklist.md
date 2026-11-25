# KB-002: Leaver (offboarding) checklist – Microsoft 365

**Audience:** Service desk · **Related ticket:** REQ0010001 / SCTASK0010001

## When to use
HR or a line manager has submitted a leaver request. Carry out the steps on the agreed leaving date and time, or **immediately** for an urgent or security-related leaver.

## Checklist

| # | Step | Where |
|---|---|---|
| 1 | Block sign-in | M365 admin center → Active users → user → Block sign-in |
| 2 | Revoke all sessions | Entra admin center → Users → user → Revoke sessions |
| 3 | Remove MFA methods | Entra admin center → user → Authentication methods |
| 4 | Convert mailbox to shared | Exchange admin center → Mailboxes → user → Others |
| 5 | Grant the manager Full Access | Exchange admin center → mailbox → Delegation |
| 6 | Set an automatic reply (if requested) | M365 admin center → user → Mail |
| 7 | Give the manager OneDrive access | M365 admin center → user → OneDrive |
| 8 | Remove from groups and distribution lists | M365 or Entra admin center → user → Groups |
| 9 | **Remove the licence (after step 4)** | M365 admin center → user → Licenses and apps |
| 10 | Wipe or retire devices, arrange hardware return | Intune admin center |

## Important
- **Always convert the mailbox to shared before removing the licence.** Removing the licence from a user mailbox starts a 30-day countdown to deletion.
- Full Access can take a few minutes to appear in the manager's Outlook.
- In **hybrid** environments, disable the account in **on-premises Active Directory**. Changes made only in the cloud are overwritten by directory sync.

## Document in the ticket
List each completed step and where it was done, then close the task as **Closed Complete**.
