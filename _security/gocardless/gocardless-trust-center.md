---
api_specs:
- filename: openapi
  format: yaml
  label: GoCardless REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://developer.gocardless.com/api-reference/openapi
certifications:
- ISO/IEC 27001
- FCA authorisation
- PCI DSS
description: GoCardless's security & compliance posture, captured from the GoCardless security page. GoCardless is ISO 27001 certified (since 2016, across all services and products) and is authorised by the UK Financial Conduct Authority under the Payment Services Regulations 2017. It handles bank-debit and open-banking payments (it does not store card PANs), and states PCI DSS compliance for the card-adjacent surface. Only certifications GoCardless states about itself are recorded here; third-party attestations are excluded.
kind: trust-center
layout: security
name: Gocardless Trust Center
name_suffix: Trust Center
overview: GoCardless maintains a public trust center documenting ISO/IEC 27001, FCA authorisation, and PCI DSS compliance.
provider_name: GoCardless
provider_slug: gocardless
slug: gocardless-trust-center
source_filename: gocardless-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-14'\nmethod: searched\nprobe: false\nsource: https://gocardless.com/security/\nurl: https://gocardless.com/security/\ndescription: >-\n  GoCardless's security & compliance posture, captured from the GoCardless\n  security page. GoCardless is ISO 27001 certified (since 2016, across all\n  services and products) and is authorised by the UK Financial Conduct\n  Authority under the Payment Services Regulations 2017. It handles bank-debit\n  and open-banking payments (it does not store card PANs), and states PCI DSS\n  compliance for the card-adjacent surface. Only certifications GoCardless\n  states about itself are recorded here; third-party attestations are excluded.\ncertifications:\n  - {name: ISO/IEC 27001, status: certified, since: '2016', scope: All GoCardless services and products, note: Reassessed annually by an accredited independent auditor (certified by the British Assessment Bureau).}\n  - {name: FCA authorisation, status: authorised, regulator:\
  \ UK Financial Conduct Authority, basis: Payment Services Regulations 2017.}\n  - {name: PCI DSS, status: compliant, note: Stated on the GoCardless security/PCI guidance; GoCardless collects bank-debit and open-banking payments and does not store card numbers.}\nreport_access:\n  note: >-\n    Security and compliance documentation (ISO 27001 certificate, due-diligence\n    packs) is provided to merchants and partners on request via GoCardless.\ndocs:\n  - https://gocardless.com/security/\n  - https://gocardless.com/faq/merchants/security/\nevidence:\n  - {source: https://gocardless.com/security/, keywords: [iso27001 certified since 2016, authorised by the uk financial conduct authority, payment services regulations 2017]}\n  - {source: https://gocardless.com/faq/merchants/security/, keywords: [pci compliant, strong encryption, safeguarded bank accounts]}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gocardless/refs/heads/main/security/gocardless-trust-center.yml
summary_line: ISO/IEC 27001, FCA authorisation, PCI DSS
tags:
- Payments
- Direct Debit
- Bank Debit
- Recurring Payments
- Subscriptions
- SEPA
- Bacs
- ACH
- Open Banking
- Fintech
trust_url: https://gocardless.com/security/
---
