# Email Delivery Ticket Example

## Overview

This document provides a sample help desk ticket for an email delivery issue. Email delivery problems may involve Outlook, Microsoft 365, DNS records, spam filtering, mailbox rules, quarantine, message trace, or sender authentication.

## Ticket Information

| Field | Details |
|---|---|
| Ticket Number | HD-1004 |
| Request Type | Incident |
| Category | Email / Microsoft 365 |
| Priority | Medium |
| Status | Escalated / Resolved |
| User | Priya Patel |
| Department | Customer Service |
| Device | LAPTOP-CS-009 |
| Email Platform | Microsoft 365 |
| Support Role | Help Desk Technician |

## Issue Summary

User reported that an expected external email was not received.

## User Impact

The user was waiting for a customer email needed to complete a service request.

## Initial User Report

```text
User stated that a customer sent an email, but it did not appear in Outlook.
User checked Inbox but could not find the message.
```

## Troubleshooting Questions

- Who sent the email?
- What time was the email sent?
- What was the sender's email address?
- What recipient address was used?
- Was there a bounce-back message?
- Does the message appear in Outlook on the web?
- Did the message go to Junk Email?
- Are other users missing external email?
- Is this one sender or multiple senders?

## Troubleshooting Steps Performed

```text
1. Confirmed the user's mailbox was accessible.
2. Tested Outlook on the web.
3. Checked Inbox, Junk Email, Deleted Items, and Archive.
4. Checked Focused and Other inbox tabs.
5. Reviewed mailbox rules with the user.
6. Checked blocked senders list.
7. Confirmed the sender address and approximate send time.
8. Sent a test email to the user from another external account.
9. Confirmed the user received the test email.
10. Escalated to Microsoft 365 administrator for message trace review.
```

## Useful Commands for DNS Checks

Check MX record:

```cmd
nslookup -type=mx company.com
```

Check SPF TXT record:

```cmd
nslookup -type=txt company.com
```

Check DMARC record:

```cmd
nslookup -type=txt _dmarc.company.com
```

## Findings

```text
The user's mailbox was active and receiving other external messages.
The missing email was not found in Inbox, Junk, Deleted Items, Archive, or mailbox rules.
A message trace was required to confirm whether the message was delivered, quarantined, rejected, or never received by Microsoft 365.
```

## Resolution

Example resolution after admin review:

```text
Microsoft 365 administrator completed message trace and confirmed the message was quarantined by spam filtering.
Admin reviewed and released the message after confirming it was legitimate.
User received the message successfully.
```

## Verification

The user confirmed:

- The released message appeared in the mailbox
- New external mail was arriving normally
- Outlook and Outlook on the web were both working

## Final Ticket Note

```text
User reported expected external customer email was missing.
Confirmed mailbox access through Outlook and Outlook on the web.
Checked Inbox, Junk Email, Deleted Items, Archive, Focused/Other inbox, and mailbox rules.
Confirmed user could receive external test email.
Escalated to Microsoft 365 admin for message trace.
Message trace confirmed email was quarantined by spam filtering.
Message was reviewed, released, and received by user.
Ticket resolved.
```

## Escalation Criteria

Escalate if:

- Message trace is required
- Quarantine review is required
- Multiple users are affected
- MX, SPF, DKIM, or DMARC records may be incorrect
- Mail flow rules may be blocking email
- Sender domain may be blocked
- Account compromise or suspicious forwarding is found
- Microsoft 365 service health issue is suspected

## Skills Demonstrated

- Email delivery troubleshooting
- Outlook and webmail testing
- Mailbox rule review
- Microsoft 365 message trace awareness
- DNS email record awareness
- Escalation documentation
