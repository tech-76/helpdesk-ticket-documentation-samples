# Password Reset Ticket Example

## Overview

This document provides a sample help desk ticket for an Active Directory or Microsoft 365 password reset request.

Password reset tickets are common in help desk and service desk roles. They must be handled securely because password resets can give access to company systems.

## Ticket Information

| Field | Details |
|---|---|
| Ticket Number | HD-1001 |
| Request Type | Service Request |
| Category | User Access |
| Priority | Medium |
| Status | Resolved |
| User | Jordan Smith |
| Department | Sales |
| System | Active Directory / Microsoft 365 |
| Device | LAPTOP-SALES-014 |
| Support Role | Help Desk Technician |

## Issue Summary

User was unable to sign in because they forgot their password.

## User Impact

The user could not access their Windows account, Microsoft 365 email, Teams, shared files, or business applications.

## Initial User Report

```text
User reported they were unable to sign in after forgetting their password.
User stated they had attempted multiple passwords and may have locked the account.
```

## Troubleshooting Questions

- Can you confirm your username or email address?
- Are you signing in to Windows, Microsoft 365, VPN, or another system?
- Did you recently change your password?
- Are you receiving an account locked message?
- Are you working onsite or remotely?
- Do you have access to your MFA device?
- Are any other users affected?

## Security Verification

Before resetting the password, the user's identity was verified according to support procedure.

Verification methods may include:

- Employee ID confirmation
- Manager confirmation
- Approved MFA confirmation
- Callback to a known phone number on file

Passwords should never be sent in plain text email or written in ticket notes.

## Troubleshooting Steps Performed

```text
1. Verified user identity using approved support process.
2. Located user account in Active Directory.
3. Confirmed the account was locked after multiple failed login attempts.
4. Unlocked the account.
5. Reset the password using a temporary password.
6. Enabled "User must change password at next logon."
7. Advised user to sign in and create a new password.
8. Confirmed user could access Windows and Microsoft 365.
9. Reviewed possible saved old passwords on phone, Outlook, and VPN.
```

## Findings

```text
The user account was locked due to multiple failed password attempts.
No wider authentication issue was identified.
The issue was limited to one user account.
```

## Resolution

```text
Unlocked the Active Directory account and reset the user password.
Required password change at next logon.
User successfully created a new password and signed in.
```

## Verification

The user confirmed access to:

- Windows workstation
- Microsoft 365
- Outlook
- Teams
- Shared folders
- VPN, if required

## Final Ticket Note

```text
Verified user identity according to support procedure.
Checked Active Directory and confirmed account was locked.
Unlocked account and reset temporary password.
Enabled password change at next logon.
User signed in successfully and confirmed Microsoft 365 access.
Reviewed saved password locations to prevent future lockouts.
Ticket resolved.
```

## Escalation Criteria

Escalate if:

- Account keeps locking repeatedly
- Suspicious login activity is detected
- MFA reset is required
- The user cannot verify identity
- Password reset does not restore access
- Multiple users report authentication issues
- Account compromise is suspected

## Security Best Practices

- Verify identity before resetting passwords.
- Never include passwords in ticket notes.
- Require users to change temporary passwords.
- Confirm MFA access.
- Watch for repeated lockouts.
- Escalate suspicious activity.
- Follow company password policy.

## Skills Demonstrated

- Password reset support
- Active Directory account unlock
- Identity verification
- Microsoft 365 access support
- Security awareness
- Ticket documentation
