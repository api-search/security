---
api_specs:
- filename: ontraport-metadata-api-openapi.yml
  format: yaml
  label: Ontraport Metadata API
  slug: ontraport-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontraport/refs/heads/main/openapi/ontraport-metadata-api-openapi.yml
- filename: ontraport-objects-api-openapi.yml
  format: yaml
  label: Ontraport Objects API
  slug: ontraport-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontraport/refs/heads/main/openapi/ontraport-objects-api-openapi.yml
certifications:
- PCI DSS
- GDPR
description: 'Ontraport has no trust center — no trust.ontraport.com, no Vanta/Drata/SafeBase portal, no downloadable attestation, no sub-processor page reachable from the public site. What it has is a marketing security page and a legal page, which between them carry two named compliance claims: PCI DSS Level 1 certification and GDPR compliance as a data processor. Both are self-asserted prose. This file records those claims and their evidence; it does not upgrade them.'
kind: trust-center
layout: security
name: Ontraport Trust Center
name_suffix: Trust Center
overview: Ontraport maintains a public trust center documenting PCI DSS and GDPR compliance.
provider_name: Ontraport
provider_slug: ontraport
slug: ontraport-trust-center
source_filename: ontraport-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://ontraport.com/features/platform/security-and-scalability/ and\n  https://ontraport.com/legal\ndescription: >-\n  Ontraport has no trust center — no trust.ontraport.com, no Vanta/Drata/SafeBase portal, no\n  downloadable attestation, no sub-processor page reachable from the public site. What it\n  has is a marketing security page and a legal page, which between them carry two named\n  compliance claims: PCI DSS Level 1 certification and GDPR compliance as a data processor.\n  Both are self-asserted prose. This file records those claims and their evidence; it does\n  not upgrade them.\ntrust_center:\n  exists: false\n  url: null\n  probed:\n  - url: https://trust.ontraport.com\n    result: redirects to https://ontraport.com/service-status (the Statuspage link), not a trust portal\n  - url: https://ontraport.com/security\n    status: 404\n  platform: none\ncertifications:\n- name: PCI DSS\n  level: Level 1\n  status:\
  \ claimed\n  claim: >-\n    \"Ontraport meets the highest level of security – PCI-DSS Level 1 Certification\"\n  source: https://ontraport.com/features/platform/security-and-scalability/\n  corroboration: >-\n    A \"PCI DSS, Level 1\" badge appears in the site footer across ontraport.com pages.\n  attestation_published: false\n  qsa: not named\n  attestation_date: not published\n  note: >-\n    Credible for a platform that processes card payments through its own gateway integrations\n    and describes an isolated payment-processing system, but it is a self-assertion — no AOC\n    or ROC summary is downloadable.\n- name: GDPR\n  role: data processor\n  status: claimed\n  claim: >-\n    \"Ontraport attests that we comply with GDPR as a Data Processor but does not and can not\n    ensure your compliance as a Data Controller.\"\n  source: https://ontraport.com/legal\n  sub_processors:\n    committed: true\n    published_url: not resolvable\n    note: >-\n      The legal page states \"We maintain\
  \ a list of sub-processors below for your review\". The\n      list is rendered inside the accordion sections of https://ontraport.com/legal rather\n      than at a stable, linkable URL.\nnot_claimed:\n- SOC 2 Type I or Type II\n- ISO/IEC 27001\n- ISO/IEC 27017 or 27018\n- HIPAA / BAA\n- FedRAMP\n- CSA STAR\n- TX-RAMP or StateRAMP\nsecurity_practices_published:\n  source: https://ontraport.com/features/platform/security-and-scalability/\n  claims:\n  - Daily off-site backups with redundancy\n  - Multi-factor authentication (SMS, email, or social login)\n  - Role-based permission management\n  - Free SSL certificates for all hosted pages\n  - Encryption of sensitive data in transit\n  - Custom-built breach response technology\n  - Payment processing isolated from the main application\n  - 24/7 systems monitoring with automated hourly tests\n  - An in-product Automation Log tracking team actions and changes\n  - Dedicated infrastructure available on enterprise accounts\n  uptime_commitment:\
  \ none published\n  data_center_locations: not published\n  pen_test_summary: not published\n  encryption_at_rest: not stated\ngaps:\n- >-\n  No SOC 2 — the single most common enterprise procurement requirement, and the one a CRM\n  holding an entire customer database is most often asked for.\n- >-\n  No trust portal, so every security question is a sales conversation rather than a\n  self-serve document.\n- >-\n  No published sub-processor list at a stable URL, despite a contractual commitment in the\n  Terms of Service to maintain one.\n- >-\n  No vulnerability disclosure policy and no security contact. See\n  security/ontraport-vulnerability-disclosure.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ontraport/refs/heads/main/security/ontraport-trust-center.yml
summary_line: PCI DSS, GDPR
tags:
- CRM
- Marketing Automation
- Email Marketing
- Ecommerce
- Landing Pages
- Membership Sites
- MCP
- AI Agents
- Payments
- Sales Automation
trust_url: ''
---
