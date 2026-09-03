---
certifications:
- SOC 2 Type II
- ISO/IEC 27001
- ISO 22301:2019
- GDPR
- 21 CFR Part 11
- EU GMP Annex 11
- ISO/IEC 17025
description: ''
kind: trust-center
layout: security
name: Uncountable Trust Center
name_suffix: Trust Center
overview: Uncountable maintains a public trust center documenting SOC 2 Type II, ISO/IEC 27001, ISO 22301:2019, GDPR, 21 CFR Part 11, EU GMP Annex 11, and ISO/IEC 17025 compliance.
provider_name: Uncountable
provider_slug: uncountable
slug: uncountable-trust-center
source_filename: uncountable-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: searched\nsource: https://www.uncountable.com/uncountable-security\nnote: >-\n  Uncountable runs no separate trust.uncountable.com portal (DNS does not resolve) and no\n  third-party trust-center host (Vanta/Drata/SafeBase) was found. Its compliance posture\n  is published on a single page on the marketing site, which does name specific\n  certifications, an issuing auditor and a certificate number — richer than most trust\n  pages of this shape. Certificates themselves are not downloadable from the page;\n  control mapping and DPAs are stated as available on request.\ntrust_center_url: https://www.uncountable.com/uncountable-security\ntrust_center_page_status: 200\ndedicated_portal: false\nportal_probes:\n- url: https://trust.uncountable.com/\n  status: 0\n  note: DNS does not resolve\ncertifications:\n- name: SOC 2 Type II\n  status: certified\n  cadence: annual external audit\n  detail: >-\n    Uncountable states the most recent report carries\
  \ no qualifications and no exceptions.\n  evidence: https://www.uncountable.com/uncountable-security\n- name: ISO/IEC 27001\n  status: certified\n  cadence: annual\n  evidence: https://www.uncountable.com/uncountable-security\n- name: ISO 22301:2019\n  status: certified\n  scope: business continuity management\n  certificate: BCMS-UN-111125\n  auditor: A-LIGN\n  accreditation: ANAB-accredited\n  valid_to: '2028-11'\n  evidence: https://www.uncountable.com/uncountable-security\n- name: GDPR\n  status: compliant\n  detail: data processing agreements available\n  evidence: https://www.uncountable.com/uncountable-security\n- name: 21 CFR Part 11\n  status: aligned\n  detail: electronic signature and audit trail capabilities aligned to the regulation\n  evidence: https://www.uncountable.com/uncountable-security\n- name: EU GMP Annex 11\n  status: aligned\n  detail: computerised systems controls aligned\n  evidence: https://www.uncountable.com/uncountable-security\n- name: ISO/IEC 17025\n  status:\
  \ in-use\n  detail: >-\n    Stated as already in use in accredited laboratories. This is an accreditation held by\n    the customer laboratory, not by Uncountable.\n  evidence: https://www.uncountable.com/uncountable-security\nframeworks:\n- name: NIST\n  status: incorporated\n  detail: specific control mapping available on request\n- name: CIS\n  status: incorporated\n  detail: specific control mapping available on request\nnot_claimed:\n- HIPAA\n- FedRAMP\n- PCI DSS\ninfrastructure:\n  hosting: Amazon Web Services\n  regions:\n  - US\n  - EU\n  - Japan\n  cdn: AWS CloudFront\n  encryption_at_rest: AES-256\n  encryption_in_transit: TLS 1.3, minimum TLS 1.2\naudit:\n  immutable_audit_trail: true\n  retention: contract lifetime\n  export_formats:\n  - CSV\n  - XLSX\n  - JSON\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uncountable/refs/heads/main/security/uncountable-trust-center.yml
summary_line: SOC 2 Type II, ISO/IEC 27001, ISO 22301:2019, GDPR, 21 CFR Part 11, EU GMP Annex 11, ISO/IEC 17025
tags:
- Company
- Laboratory Informatics
- LIMS
- Electronic Lab Notebook
- R&D Data Management
- Product Lifecycle Management
- Quality Management
- Materials Science
- Chemicals
- Artificial Intelligence
- Model Context Protocol
trust_url: ''
---
