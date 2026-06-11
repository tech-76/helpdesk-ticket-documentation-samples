# VPN Connection Ticket Example

## Overview

This document provides a sample help desk ticket for a VPN connection issue. VPN troubleshooting is common when supporting remote and hybrid users.

VPN issues may involve internet connectivity, password problems, MFA, saved credentials, DNS, routing, permissions, or VPN client configuration.

## Ticket Information

| Field | Details |
|---|---|
| Ticket Number | HD-1003 |
| Request Type | Incident |
| Category | Network / VPN |
| Priority | Medium |
| Status | Resolved |
| User | Daniel Lee |
| Department | Operations |
| Device | LAPTOP-OPS-018 |
| Location | Remote |
| VPN Client | Company VPN Client |
| Support Role | Help Desk Technician |

## Issue Summary

User could connect to the internet but could not connect to the company VPN.

## User Impact

The user could not access shared drives, internal applications, or company network resources while working remotely.

## Initial User Report

```text
User reported that VPN failed to connect and showed an authentication error.
User confirmed home internet was working.
```

## Troubleshooting Questions

- Does your internet work without VPN?
- What error message appears?
- Did you recently change your password?
- Are you receiving an MFA prompt?
- Are you using the correct VPN profile?
- Can you sign in to Microsoft 365 or webmail?
- Is this happening on one device only?
- Are other remote users affected?

## Troubleshooting Steps Performed

```text
1. Confirmed user was working remotely.
2. Confirmed internet access worked without VPN.
3. Asked user to sign in to Microsoft 365 webmail to confirm password.
4. Confirmed password worked in webmail.
5. Checked whether user received MFA prompt.
6. Confirmed user was selecting correct VPN profile.
7. Restarted VPN client.
8. Removed old saved VPN credentials from Credential Manager.
9. Asked user to reconnect using current password.
10. Confirmed MFA prompt was approved.
11. Verified VPN connected successfully.
12. Tested access to internal shared drive.
```

## Useful Commands Used

Check IP configuration:

```cmd
ipconfig /all
```

Test internet access:

```cmd
ping 8.8.8.8
ping google.com
```

Test internal DNS after VPN connection:

```cmd
nslookup fileserver01.company.local
```

Open Credential Manager:

```cmd
control keymgr.dll
```

## Findings

```text
The user's internet connection was working.
The VPN client was using an old saved password after a recent password change.
After removing saved credentials, the user was able to authenticate successfully.
```

## Resolution

```text
Removed outdated saved VPN credentials from Windows Credential Manager.
User reconnected to VPN using current password and completed MFA.
Internal network access was restored.
```

## Verification

The user confirmed access to:

- VPN connection
- Internal shared drive
- Company intranet
- Required business application

## Final Ticket Note

```text
User reported VPN authentication failure while working remotely.
Confirmed internet connection was working and Microsoft 365 sign-in was successful.
Reviewed VPN sign-in process and confirmed user recently changed password.
Removed old saved VPN credentials from Credential Manager.
User reconnected using current password and approved MFA prompt.
Confirmed access to internal shared drive and intranet.
Ticket resolved.
```

## Escalation Criteria

Escalate if:

- Multiple users cannot connect to VPN
- VPN server or gateway may be down
- MFA reset is required
- User is missing VPN security group access
- VPN certificate is expired
- Internal DNS fails after connection
- Routing issue is suspected
- Account compromise is suspected

## Skills Demonstrated

- VPN troubleshooting
- Remote user support
- Credential Manager awareness
- MFA support awareness
- DNS testing
- Internal resource testing
- Ticket documentation
