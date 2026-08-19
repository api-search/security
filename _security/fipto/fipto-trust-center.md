---
api_specs:
- filename: fipto-customer-api-openapi.yml
  format: yaml
  label: Fipto API
  slug: customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fipto/refs/heads/main/openapi/fipto-customer-api-openapi.yml
certifications:
- ISO/IEC 27001:2022
description: ''
kind: trust-center
layout: security
name: Fipto Trust Center
name_suffix: Trust Center
overview: Fipto maintains a public trust center documenting ISO/IEC 27001:2022 compliance.
provider_name: Fipto
provider_slug: fipto
slug: fipto-trust-center
source_filename: fipto-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nprobe: true\nurl: https://www.fipto.com/company/compliance\nalso: https://www.fipto.com/company/security\nnote: >-\n  Fipto runs no third-party trust portal (trust.fipto.com and security.fipto.com do not resolve), but\n  it publishes two first-party pages that serve the same purpose and name real certifications and\n  licence numbers: a Compliance Center and a Security Center. The mechanical probe\n  (probe-security-programs.py) missed both because it only checks /trust, /security and /compliance at\n  the domain root — Fipto serves them under /company/. Recorded here from a direct read.\ncertifications: ['ISO/IEC 27001:2022']\nlicences:\n- 'Payment Institution — ACPR (Banque de France), CIB 17908'\n- 'MiCA CASP — AMF (France), authorisation A2026-009'\n- 'VASP registration — Luxembourg'\ncontrols_published:\n- 100% segregation of client funds\n- Regular third-party penetration testing\n- 24/7 infrastructure monitoring and alerting\n\
  - Multi-factor authentication, multi-signature validation, role-based permissions, session timeouts\n- End-to-end encryption in transit and at rest\n- Daily backups, quarterly recovery testing, automated failover, redundant cloud hosting\n- GDPR-aligned data deletion policies\n- Mandatory KYC/KYB for AML/CFT and sanctions compliance\npolicies:\n- {name: Custody / Conservation Policy, url: 'https://www.fipto.com/legal/conservation-policy'}\n- {name: Order Execution Policy, url: 'https://www.fipto.com/legal/order-execution-policy'}\n- {name: Conflict of Interest Policy, url: 'https://www.fipto.com/legal/conflict-of-interest-policy'}\n- {name: Complaints, url: 'https://www.fipto.com/legal/complaints'}\n- {name: Terms and Conditions, url: 'https://www.fipto.com/legal/terms-and-conditions'}\n- {name: Privacy Policy, url: 'https://www.fipto.com/legal/privacy'}\nevidence:\n- {source: 'https://www.fipto.com/company/compliance', http_status: 200,\n   keywords: [mica, casp, acpr, payment institution,\
  \ 'iso/iec 27001:2022', aml/cft, compliance center]}\n- {source: 'https://www.fipto.com/company/security', http_status: 200,\n   keywords: [iso 27001, penetration testing, segregated, encryption, mfa]}\n- {source: 'https://trust.fipto.com', http_status: 0, note: does not resolve}\n- {source: 'https://security.fipto.com', http_status: 0, note: does not resolve}\nvulnerability_disclosure:\n  published: false\n  note: >-\n    Neither page — nor any page in the sitemap — publishes a vulnerability disclosure policy, a bug\n    bounty program, a responsible-disclosure address or a security@ contact, and\n    /.well-known/security.txt returns 404 on every host. For an ISO 27001-certified, dual-licensed\n    payment institution this is the most conspicuous gap in an otherwise strong posture. No\n    `Security` or `VulnerabilityDisclosure` pointer is emitted in apis.yml, because there is nothing\n    published to point at.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fipto/refs/heads/main/security/fipto-trust-center.yml
summary_line: ISO/IEC 27001:2022
tags:
- Company
- Blockchain
- Payments
- Stablecoins
- Banking
- Treasury
- Cross-Border Payments
- Digital Currency
- Fintech
- Wallets
trust_url: https://www.fipto.com/company/compliance
---
