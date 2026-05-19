---
title: kdc-ap-automation — Launch
---

# kdc-ap-automation

This is an internal accounts-payable automation tool operated by Kristen
Distributing Company ("KDC"). It is not offered to the general public.

## What it does

The tool reads vendor invoice PDFs uploaded by KDC accounting staff,
extracts the invoice fields automatically, and posts the resulting Bill
into KDC's QuickBooks Online company with the original PDF attached for
audit reference.

## Access

Access is restricted to authorized KDC accounting and IT personnel. The
tool runs as a command-line application on KDC-managed workstations. There
is no public web interface.

## Connection management

The connection between this tool and QuickBooks Online is authorized once,
during initial setup, by KDC IT using Intuit's standard OAuth flow. After
that, the tool refreshes its access token automatically as long as the
authorization remains valid in QuickBooks Online.

To revoke access at any time, see the [Disconnect](disconnect.html) page.

## Documents

- [End-User License Agreement](eula.html)
- [Privacy Policy](privacy.html)

## Contact

luke.arpey@kristendistributing.com
