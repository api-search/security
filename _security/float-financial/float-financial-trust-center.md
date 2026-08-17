---
api_specs:
- filename: float-financial-openapi.yml
  format: yaml
  label: Float Public API
  slug: float-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/float-financial/refs/heads/main/openapi/float-financial-openapi.yml
certifications:
- SOC 2 Type 2
- PCI DSS
description: ''
kind: trust-center
layout: security
name: Float Financial Trust Center
name_suffix: Trust Center
overview: Float Financial maintains a public trust center documenting SOC 2 Type 2 and PCI DSS compliance.
provider_name: Float Financial
provider_slug: float-financial
slug: float-financial-trust-center
source_filename: float-financial-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: searched\nsource: https://trust.floatfinancial.com/ (HTTP 200) and https://floatfinancial.com/security (HTTP 200)\ntrust_center:\n  published: true\n  url: https://trust.floatfinancial.com/\n  status: 200\n  title: Float Trust Center\n  platform: Vanta\n  platform_evidence: >-\n    The page ships Vanta's `vanta-entry-loader` bundle and its og:image is served from\n    https://app.vanta.com/doc?s=u2ulatlqovjbfdmujaky. Content is client-rendered, so certification detail was\n    read from Float's own security page rather than scraped from the JS shell.\n  document_access: request-based\n  note: >-\n    \"You can request a copy of our SOC 2 Report at our Trust Centre.\" — https://floatfinancial.com/security.\n    Reports are gated behind a request form on the Vanta trust centre; the certification claims themselves are\n    published openly on floatfinancial.com/security.\ncertifications:\n- name: SOC 2 Type 2\n  status: certified\n  scope: Information\
  \ security practices, audited annually\n  report_available: on request via trust centre\n  source: https://floatfinancial.com/security\n- name: PCI DSS\n  status: certified\n  scope: Cardholder data protection — storage, processing and transmission\n  report_available: on request via trust centre\n  source: https://floatfinancial.com/security\nregulatory:\n- name: RPAA (Retail Payment Activities Act)\n  status: Registered payment services provider (PSP)\n  jurisdiction: Canada\n  detail: Customer deposits held in segregated trust accounts at Canadian financial institutions, never commingled.\n  source: https://floatfinancial.com/security\n- name: Payments Canada\n  status: Member\n  jurisdiction: Canada\n  source: https://floatfinancial.com/security\n- name: CDIC\n  status: Deposit insurance through banking partner\n  jurisdiction: Canada\n  detail: Float is a financial technology company, not a bank.\n  source: https://floatfinancial.com/security\nsecurity_page: https://floatfinancial.com/security\n\
  security_contact: security@floatfinancial.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/float-financial/refs/heads/main/security/float-financial-trust-center.yml
summary_line: SOC 2 Type 2, PCI DSS
tags:
- spend-management
- corporate-cards
- expense-management
- accounts-payable
- bill-pay
- reimbursements
- business-banking
- accounting-integration
- fintech
- canada
- payments
- erp-integration
trust_url: ''
---
