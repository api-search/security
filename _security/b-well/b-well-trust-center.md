---
api_specs:
- filename: b-well-users-api-openapi.yml
  format: yaml
  label: b.well Users API
  slug: b-well-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/b-well/refs/heads/main/openapi/b-well-users-api-openapi.yml
- filename: b-well-webhook-api-openapi.yml
  format: yaml
  label: b.well Webhook API
  slug: b-well-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/b-well/refs/heads/main/openapi/b-well-webhook-api-openapi.yml
certifications:
- HITRUST
- NIST Cybersecurity Framework (CSF)
- HIPAA
description: ''
kind: trust-center
layout: security
name: B Well Trust Center
name_suffix: Trust Center
overview: b.well maintains a public trust center documenting HITRUST, NIST Cybersecurity Framework (CSF), and HIPAA compliance.
provider_name: b.well
provider_slug: b-well
slug: b-well-trust-center
source_filename: b-well-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: searched\nsource: https://www.icanbwell.com/health-data-security-for-consumers/\nurl: https://www.icanbwell.com/health-data-security-for-consumers/\nname: b.well Health Data Security\ndetail: >-\n  b.well does not operate a hosted trust center (no trust.icanbwell.com — TLS\n  handshake fails — and no /security/ or /trust/ page on the corporate site). It\n  publishes its security and compliance posture as a narrative page on its own domain,\n  which names the certifications below and describes the audit cadence behind them.\ncertifications:\n- HITRUST\n- NIST Cybersecurity Framework (CSF)\n- HIPAA\nframeworks:\n- name: CARIN Alliance Trust Framework and Code of Conduct\n  voluntary: true\n  detail: >-\n    b.well states it \"voluntarily follows the CARIN Alliance Trust Framework and Code\n    of Conduct\" — the consumer-directed health data exchange code of conduct, which is\n    the relevant governance layer for a consumer-mediated network.\n\
  audit:\n  cadence: annual security reviews; independent external verification at least biennially\n  quote: >-\n    \"Our systems are subject to annual security reviews and have achieved HITRUST and\n    US NIST cybersecurity framework (CSF) certification, which require independent\n    verification of our security-related policies, procedures, and implemented controls\n    by external auditors on at least a biennial (2 year) basis.\"\nencryption:\n  quote: >-\n    \"Your data is encrypted in secure servers, not stored on your local device; and\n    always encrypted during transmissions.\"\n  at_rest: true\n  in_transit: true\ngaps:\n- No downloadable or gated report portal (no SOC 2 / HITRUST report request flow published).\n- No report date, scope statement or auditor named, so the currency of each certification\n  cannot be verified from the public page.\n- SOC 2 is claimed for the bailey product in press material but is not asserted on b.well's\n  own security page, so it is NOT recorded\
  \ as a certification here.\nevidence:\n- source: https://www.icanbwell.com/health-data-security-for-consumers/\n  keywords:\n  - hitrust\n  - nist cybersecurity framework\n  - hipaa\n  - carin alliance\nx-evidence:\n  fetched: '2026-08-15'\n  evidence:\n  - url: https://www.icanbwell.com/health-data-security-for-consumers/\n    status: 200\n  - url: https://www.icanbwell.com/security/\n    status: 404\n  - url: https://www.icanbwell.com/trust/\n    status: 404\n  - url: https://trust.icanbwell.com/\n    status: 0\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/b-well/refs/heads/main/security/b-well-trust-center.yml
summary_line: HITRUST, NIST Cybersecurity Framework (CSF), HIPAA
tags:
- Company
- Health
- Healthcare
- Digital Health
- FHIR
- Health Data
- Interoperability
- Patient Access
- Health Records
- Model Context Protocol
trust_url: https://www.icanbwell.com/health-data-security-for-consumers/
---
