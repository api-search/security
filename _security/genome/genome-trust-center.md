---
api_specs:
- filename: genome-host-to-host-api-openapi.yml
  format: yaml
  label: Genome Host-to-Host API
  slug: genome-host-to-host-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genome/refs/heads/main/openapi/genome-host-to-host-api-openapi.yml
- filename: genome-payouts-api-openapi.yml
  format: yaml
  label: Genome Payouts API
  slug: genome-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genome/refs/heads/main/openapi/genome-payouts-api-openapi.yml
certification_count: 3
certifications:
- ISO/IEC 27001:2022
- ISO/IEC 27701:2019
- PCI DSS
description: ''
kind: trust-center
layout: security
name: Genome Trust Center
name_suffix: Trust Center
overview: Genome maintains a public trust center documenting ISO/IEC 27001:2022, ISO/IEC 27701:2019, and PCI DSS compliance.
provider_name: Genome
provider_slug: genome
slug: genome-trust-center
source_filename: genome-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: searched\nsource: https://genome.eu/genome-security/ + the certificate PDFs it links on cdn.genome.eu\nprovider: Genome\nproviderId: genome\ntrust_center:\n  url: https://genome.eu/genome-security/\n  probed: '2026-09-12'\n  http_status: 200\n  dedicated_portal: false\n  note: >-\n    Genome has no trust portal in the Vanta/Drata sense — no document request flow, no subprocessor\n    list, no live control status. What it has is better than a badge wall and worse than a portal: the\n    two ISO certificates are published as downloadable PDFs that name the certifying body, the\n    registration number and the validity window, so a buyer can verify them against the registrar\n    without asking anyone.\ncertifications:\n- name: ISO/IEC 27001:2022\n  status: certified\n  holder: Maneuver LT, UAB\n  scope: Provision of electronic money and payment services\n  statement_of_applicability: v1.3, dated 2024-10-24\n  body: TUV NORD CERT GmbH\n  registration_no:\
  \ 44 121 24 32 0215\n  audit_report_no: 35924 2167\n  valid_from: '2024-12-20'\n  valid_until: '2027-12-19'\n  initial_certification: '2024'\n  document: https://cdn.genome.eu/certificate_27001_f47cad0aca.pdf\n- name: ISO/IEC 27701:2019\n  status: certified\n  holder: Maneuver LT, UAB\n  scope: >-\n    Provision of electronic money and payment services; the organisation acts as PII controller and\n    PII processor. Valid only in conjunction with the ISO/IEC 27001 certificate above.\n  statement_of_applicability: v1.3, dated 2024-10-24\n  body: TUV CYPRUS LTD\n  registration_no: '49254012501'\n  audit_report_no: '05022025'\n  valid_from: '2025-02-14'\n  valid_until: '2028-02-13'\n  initial_certification: '2025'\n  document: https://cdn.genome.eu/certificate_27701_b2b0eb0698.pdf\n- name: PCI DSS\n  status: claimed\n  note: >-\n    \"Our team works with PCI DSS-aligned standards.\" No AoC, level or assessor is published. Genome\n    also displays a PCI logotype on the security page. Treated\
  \ as a claim, not a certification.\nregulatory:\n  entity: UAB \"Maneuver LT\"\n  licence: Electronic Money Institution\n  supervisor: Bank of Lithuania (Lietuvos bankas)\n  supervisor_url: https://www.lb.lt\n  source: https://genome.eu/legal-regulations/\n  frameworks_named:\n  - DORA (Digital Operational Resilience Act)\n  - PSD2\n  - GDPR (via the ISO/IEC 27701 PIMS scope and https://genome.eu/privacy-notice/)\nsecurity_practices_published:\n- Two-factor authentication on transfers\n- Strong Customer Authentication on online card payments\n- Encryption and tokenization of card data\n- Transaction monitoring\n- Real-time transaction visibility and in-app card controls\nfraud_reporting:\n  email: fraud@genome.eu\n  alternate: support@genome.eu\n  note: >-\n    This is an ACCOUNT fraud channel for customers, not a vulnerability disclosure channel for\n    researchers — Genome's instruction is to block the card or account in the app first and then write.\nvulnerability_disclosure:\n  program:\
  \ none found\n  security_txt: absent on all seven hosts (probed 2026-09-12)\n  bug_bounty: none found on HackerOne, Bugcrowd or Intigriti\n  policy_page: none found\n  note: >-\n    A researcher who finds a flaw in a licensed EMI has no published route in. No Security pointer is\n    wired into apis.yml, because there is nothing to point at.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genome/refs/heads/main/security/genome-trust-center.yml
summary_line: ISO/IEC 27001:2022, ISO/IEC 27701:2019, PCI DSS
tags:
- Finance
- Payments
- Banking
- Open Banking
- PSD2
- SEPA
- Card Processing
- Payouts
- Electronic Money Institution
- Europe
trust_url: ''
---
