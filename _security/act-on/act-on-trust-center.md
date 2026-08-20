---
api_specs:
- filename: act-on-rest-api-openapi.yml
  format: yaml
  label: Act-On REST API
  slug: act-on-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/act-on/refs/heads/main/openapi/act-on-rest-api-openapi.yml
- filename: act-on-custom-objects-service-openapi.yml
  format: yaml
  label: Act-On Custom Objects Service
  slug: act-on-custom-objects-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/act-on/refs/heads/main/openapi/act-on-custom-objects-service-openapi.yml
certifications:
- ISO 27001
- HIPAA
- TX-RAMP
- TRUSTe
description: ''
kind: trust-center
layout: security
name: Act On Trust Center
name_suffix: Trust Center
overview: Act-On maintains a public trust center documenting ISO 27001, HIPAA, TX-RAMP, and TRUSTe compliance.
provider_name: Act-On
provider_slug: act-on
slug: act-on-trust-center
source_filename: act-on-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://act-on.com/certifications-associations/\napi: Act-On platform\nsummary: >-\n  Act-On publishes a Certifications & Associations page naming four security and\n  privacy credentials plus its trade-association memberships. It is a marketing-page\n  list, not a trust center: there is no evidence portal, no report request flow, no\n  certificate numbers, no auditor named, no dates, and no subprocessor list on the\n  page.\ntrust_center:\n  exists: false\n  url: null\n  note: >-\n    No trust.act-on.com, no security portal, and no /security, /trust,\n    /security-and-compliance or /company/security page — act-on.com answers 200 with\n    the homepage for every unknown path (415,734-byte soft 404), so those 200s are\n    not documents. The certifications page below is the closest published surface.\ncertifications_page: https://act-on.com/certifications-associations/\ncertifications:\n- name: ISO 27001\n  scope: Act-On Software\
  \ information security management system\n  status: certified\n  first_earned: '2022'\n  certificate_id: null\n  auditor: null\n  evidence: Named on https://act-on.com/certifications-associations/; announced at\n    https://act-on.com/learn/news-press/act-on-software-obtains-industry-leading-security-certification/\n- name: HIPAA\n  scope: Marketing automation platform; Act-On states it maintains compliance with\n    the HIPAA security rule\n  status: compliant\n  certificate_id: null\n  auditor: null\n  evidence: Named on https://act-on.com/certifications-associations/; announced at\n    https://act-on.com/learn/news-press/act-on-software-hipaa-compliance-iso-27001-certification/\n- name: TX-RAMP\n  scope: Texas state agency cloud services\n  status: certified\n  certificate_id: null\n  evidence: Named on https://act-on.com/certifications-associations/\n- name: TRUSTe\n  scope: Privacy program seal\n  status: certified\n  certificate_id: null\n  evidence: Named on https://act-on.com/certifications-associations/\n\
  claims_not_first_party:\n- name: SOC 2\n  status: unverified\n  note: >-\n    Third-party summaries and Act-On blog copy describe the DATA CENTER that hosts\n    Act-On as SOC 2 compliant. SOC 2 does not appear on Act-On's own Certifications &\n    Associations page as an Act-On attestation, so it is recorded here as a\n    facility-level claim, not an Act-On certification. Not counted above.\nassociations:\n- Direct Marketing Association (DMA)\n- Direct Marketing Association UK (DMA UK)\n- Email Sender and Provider Coalition (ESPC)\n- Oregon Entrepreneurs Network (OEN)\nlegal:\n  terms_of_service: https://act-on.com/terms-of-service/\n  privacy_policy: https://act-on.com/privacy-policy/\n  data_processing_addendum: https://act-on.com/data-processing-addendum/\n  accessibility_statement: https://act-on.com/accessibility-statement-audioeye-trusted/\n  support_terms_pdf: https://act-on.com/wp-content/uploads/2023/02/Support-Terms-and-Conditions_2023-1.pdf\ngaps:\n- No SOC 2 report or ISO\
  \ certificate is offered for download or under NDA request.\n- No subprocessor list published at a stable URL.\n- No penetration-test summary or security whitepaper linked from the certifications\n  page.\n- No vulnerability disclosure policy — see security/act-on-vulnerability-disclosure.yml.\nprobes:\n- url: https://act-on.com/certifications-associations/\n  status: 200\n- url: https://act-on.com/trust/\n  status: 200\n  note: soft 404 — returns the 415,734-byte homepage\n- url: https://act-on.com/security/\n  status: 200\n  note: soft 404 — returns the 415,734-byte homepage\n- url: https://act-on.com/security-and-compliance/\n  status: 200\n  note: soft 404 — returns the 415,734-byte homepage\n- url: https://act-on.com/terms-of-service/\n  status: 200\n- url: https://act-on.com/privacy-policy/\n  status: 200\n- url: https://act-on.com/data-processing-addendum/\n  status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/act-on/refs/heads/main/security/act-on-trust-center.yml
summary_line: ISO 27001, HIPAA, TX-RAMP, TRUSTe
tags:
- Company
- Marketing
- Marketing Automation
- Email Marketing
- Email
- Marketing Technology
- Lead Generation
- Campaign Management
- Customer Data
- Webhook
trust_url: ''
---
