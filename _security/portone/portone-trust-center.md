---
api_specs:
- filename: portone-openapi.yml
  format: yaml
  label: PortOne Payments API (V2)
  slug: portone-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-openapi.yml
- filename: portone-openapi.yml
  format: yaml
  label: PortOne Billing Keys API (V2)
  slug: portone-billing-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-openapi.yml
- filename: portone-openapi.yml
  format: yaml
  label: PortOne Payment Schedule API (V2)
  slug: portone-payment-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-openapi.yml
- filename: portone-openapi.yml
  format: yaml
  label: PortOne Identity Verification API (V2)
  slug: portone-identity-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-openapi.yml
- filename: portone-openapi.yml
  format: yaml
  label: PortOne Cash Receipts API (V2)
  slug: portone-cash-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-openapi.yml
- filename: portone-openapi.yml
  format: yaml
  label: PortOne B2B Tax Invoice API (V2)
  slug: portone-b2b-tax-invoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-openapi.yml
- filename: portone-openapi.yml
  format: yaml
  label: PortOne Platform Partner Settlement API (V2)
  slug: portone-platform-partner-settlement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-openapi.yml
- filename: portone-openapi.yml
  format: yaml
  label: PortOne Payment Sessions & Checkout API (V2)
  slug: portone-payment-sessions-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-openapi.yml
- filename: portone-openapi.yml
  format: yaml
  label: PortOne Payment Reconciliation API (V2)
  slug: portone-payment-reconciliation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/openapi/portone-openapi.yml
certifications:
- PCI DSS
- ISMS
description: ''
kind: trust-center
layout: security
name: Portone Trust Center
name_suffix: Trust Center
overview: PortOne maintains a public trust center documenting PCI DSS and ISMS compliance.
provider_name: PortOne
provider_slug: portone
slug: portone-trust-center
source_filename: portone-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nprobe: true\nsource: https://portone.io/\nurl: https://portone.io/\ncertifications:\n- PCI DSS\n- ISMS\ncompliance_context: >-\n  PortOne operates as a licensed Korean payment orchestration / PG-adjacent\n  provider and is therefore in PCI DSS scope for handling cardholder data, and\n  is subject to Korean ISMS (Information Security Management System) and PIPA\n  (Personal Information Protection Act) obligations for identity verification\n  and personal data. Specific certification levels and current attestation dates\n  were not machine-verifiable from a public trust-center page at generation time\n  and should be reconciled against PortOne's official security materials.\nreconciled: false\nevidence:\n- source: https://portone.io/\n  keywords:\n  - payment\n  - security\n  - pci dss\n- source: openapi/portone-openapi.yml\n  keywords:\n  - identity-verifications\n  - b2b tax invoice\n  note: >-\n    Card, identity-verification, and\
  \ tax-invoice surfaces confirm regulated\n    financial-data handling consistent with PCI DSS and Korean ISMS-P scope.\nnotes: >-\n  No dedicated public trust-center portal (e.g. a SOC 2 / ISO evidence room) was\n  located during the review; certifications listed reflect the regulatory posture\n  documented for Korean payment gateways and PortOne's marketing. Treat as\n  unreconciled until confirmed against a first-party attestation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/portone/refs/heads/main/security/portone-trust-center.yml
summary_line: PCI DSS, ISMS
tags:
- Payments
- Payment Orchestration
- Fintech
- Korea
- Billing
- Identity Verification
trust_url: https://portone.io/
---
