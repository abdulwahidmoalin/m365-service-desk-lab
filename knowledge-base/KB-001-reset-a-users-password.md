# KB-001: Reset a user's Microsoft 365 password

**Audience:** Service desk · **Applies to:** Microsoft 365 admin center · **Related ticket:** INC0010002

## When to use
A user has forgotten their password or is locked out of Microsoft 365.

## Before you start
**Verify the caller's identity** using your organisation's verification process (for example, full name plus department or employee ID checked against Entra ID). Do not reset a password until identity is confirmed.

## Steps
1. Go to **admin.microsoft.com → Users → Active users**.
2. Select the user, then click **Reset password**.
3. Leave **Automatically create a password** ticked.
4. Leave **Require this user to change their password when they first sign in** ticked.
5. Click **Reset password**.
6. Give the temporary password to the user **verbally or through an approved secure channel**. Do not email it to the user's own mailbox.
7. Stay on the line while the user signs in and sets a new password.

## Document in the ticket
- How identity was verified
- That the password was reset with a forced change at next sign-in
- That the user confirmed successful sign-in
- **Never** write the password in the ticket

## If it doesn't work
- **User still can't sign in:** check the user's sign-in status isn't **blocked** and that they have a licence.
- **Blocked after sign-in:** check the **Entra ID sign-in logs** for a Conditional Access or MFA failure.
- **Repeated lockouts:** recommend **self-service password reset (SSPR)**.
