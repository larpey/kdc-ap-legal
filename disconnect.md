---
title: kdc-ap-automation — Disconnect
---

# Disconnecting kdc-ap-automation from QuickBooks Online

If you need to revoke the connection between kdc-ap-automation and KDC's
QuickBooks Online company, you can do so in two equivalent ways.

## Option A — Disconnect from inside QuickBooks Online

1. Sign in to QuickBooks Online as a company administrator.
2. Go to **Apps** → **My Apps**.
3. Find **kdc-ap-automation** in the list.
4. Click the gear icon next to it and choose **Disconnect**.

After disconnect, the tool's refresh token becomes invalid and the
local credential cache stops working. Re-authorization requires a new
OAuth flow performed by KDC IT.

## Option B — Contact KDC IT

Email luke.arpey@kristendistributing.com and request that the kdc-ap-automation
QuickBooks connection be revoked. IT will perform the disconnect and confirm
that the tool can no longer post Bills to the company.

## After disconnect

- The tool will stop posting new Bills to QuickBooks Online immediately.
- Bills already posted remain in QuickBooks Online and are not removed.
- The local SQLite state database on the operator's machine retains its
  history but cannot create new Bills until the connection is re-authorized.

## Contact

luke.arpey@kristendistributing.com
