---
title: Privacy Policy
---

# Privacy Policy

**Effective date:** 2026-05-19
**Product:** KDC-GL-AUTOMATION
**Operator:** Kristen Distributing Company ("KDC")

KDC-GL-AUTOMATION is an internal accounts-payable automation tool used by
KDC employees. This Privacy Policy explains what data the tool handles,
how it is used, and with whom it is shared.

## 1. Scope

This tool is for internal KDC use only. It does not collect data from
members of the general public.

## 2. Data handled

The tool processes:

- **Vendor invoice PDFs** uploaded by KDC AP staff, including supplier
  name, invoice number, line items, totals, dates, permit numbers, and
  any other content printed on the invoice.
- **QuickBooks Online accounting data** retrieved from KDC's QuickBooks
  Online company (vendor records, chart of accounts, existing Bills).
- **OAuth credentials** for KDC's QuickBooks Online company, stored
  locally on the operating user's machine.

No personal data of customers or members of the public is collected.

## 3. How data is used

- Extracted invoice fields are used to create matching Bill records in
  QuickBooks Online.
- The original PDF is attached to the corresponding QuickBooks Bill for
  audit and reference.
- Records of processed invoices are stored locally (SQLite) for
  idempotency and review.

## 4. Third-party processing

Data is shared with the following service providers strictly to perform
the tool's function:

- **Anthropic** — invoice PDFs are sent to Anthropic's Claude API for
  automated field extraction. See: https://www.anthropic.com/legal/privacy
- **Intuit** — Bill records and PDF attachments are written to KDC's
  QuickBooks Online company. See: https://www.intuit.com/privacy/

No data is sold, rented, or shared with any party other than the above.

## 5. Retention

- QuickBooks Bill records and attachments are retained in QuickBooks
  Online subject to KDC's normal accounting retention policy.
- Local extraction records (SQLite) and credential caches are retained
  indefinitely on the operator's machine until deleted by IT.
- Anthropic and Intuit retain data subject to their own policies linked
  above.

## 6. Security

- OAuth credential cache files are stored with restricted permissions
  (`0600`, owner read/write only).
- Secrets (`.env` file) are excluded from source control.
- Access to the tool is limited to authorized KDC personnel.

## 7. Contact

Questions about this Privacy Policy should be directed to:
luke.arpey@kristendistributing.com
