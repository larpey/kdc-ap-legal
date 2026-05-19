---
title: kdc-ap-automation — Connect
---

# Connecting kdc-ap-automation to QuickBooks Online

kdc-ap-automation is an internal accounts-payable automation tool operated
by Kristen Distributing Company ("KDC"). It is authorized once per
QuickBooks Online company by KDC IT and runs offline thereafter; it does
not provide a public "Connect to QuickBooks" button.

## How connection works

1. KDC IT performs the initial OAuth authorization using Intuit's standard
   OAuth flow against the KDC QuickBooks Online company.
2. The resulting refresh token is stored locally on the operator's
   workstation in a credential cache with restricted file permissions.
3. The tool refreshes its access token automatically as long as the
   authorization remains valid in QuickBooks Online.

## Reconnecting

If the refresh token is revoked or expires (Intuit refresh tokens expire
after approximately 100 days of inactivity), KDC IT re-runs the OAuth
authorization flow and the tool resumes normal operation.

## Requesting access

This tool is restricted to authorized KDC accounting and IT personnel.
Members of the public cannot connect to it.

If you are a KDC employee who needs access or believes the connection
should be (re)established, contact:

luke.arpey@kristendistributing.com

## Related

- [Launch / About](launch.html)
- [Disconnect](disconnect.html)
