---
api_specs:
- filename: dailypay-rest-openapi-original.yml
  format: yaml
  label: DailyPay Rest API
  slug: dailypay-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dailypay/refs/heads/main/openapi/dailypay-rest-openapi-original.yml
certifications:
- SOC 2
- ISO 27001
- PCI DSS
description: ''
kind: trust-center
layout: security
name: Dailypay Trust Center
name_suffix: Trust Center
overview: DailyPay maintains a public trust center documenting SOC 2, ISO 27001, and PCI DSS compliance.
provider_name: DailyPay
provider_slug: dailypay
slug: dailypay-trust-center
source_filename: dailypay-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nprobe: true\nsource: https://www.dailypay.com/security/\nurl: https://trust.dailypay.com/\nsecurity_page: https://www.dailypay.com/security/\ncompliance_page: https://www.dailypay.com/en-us/legal/compliance/\ncertifications:\n- SOC 2\n- ISO 27001\n- PCI DSS\ncertification_detail:\n- name: PCI DSS Level 1\n  auditor: A-Lign\n  source: https://www.dailypay.com/security/\n- name: SOC 2 Type 2\n  framework: AICPA SOC\n  source: https://www.dailypay.com/security/\n- name: ISO 27001\n  auditor: A-Lign\n  source: https://www.dailypay.com/security/\ntrust_center:\n  url: https://trust.dailypay.com/\n  http_status: 200\n  platform: HyperComply\n  note: >-\n    trust.dailypay.com resolves to a HyperComply-hosted trust center. The page renders client-side,\n    so the document inventory behind it (SOC 2 report, ISO certificate, pen-test summaries,\n    security questionnaires) could not be enumerated anonymously — access to those artefacts is\n\
  \    typically request- or NDA-gated.\npci_scope:\n  note: >-\n    DailyPay states that its Payments (card tokenization) server is its ONLY PCI-compliant API, and\n    that DailyPay handles card data only during encryption and tokenization. The corresponding\n    operation is createGenericCardToken (POST /cards/generic); the Debit Card Tokenization Element\n    is the no-code equivalent.\n  source: https://developer.dailypay.com/products/rest/guides/payments\nvulnerability_disclosure: security/dailypay-vulnerability-disclosure.yml\nevidence:\n- source: https://www.dailypay.com/security/\n  http_status: 200\n  fetched: '2026-08-01'\n  keywords:\n  - soc 2\n  - iso 27001\n  - pci dss\n  - a-lign\n- source: https://trust.dailypay.com/\n  http_status: 200\n  fetched: '2026-08-01'\n  keywords:\n  - trust center\n  - hypercomply\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dailypay/refs/heads/main/security/dailypay-trust-center.yml
summary_line: SOC 2, ISO 27001, PCI DSS
tags:
- Company
- Payments
- Payroll
- Human Resources
- Earned Wage Access
- On-Demand Pay
- Financial Services
- Fintech
- Money Transfer
- Benefits
trust_url: https://trust.dailypay.com/
---
