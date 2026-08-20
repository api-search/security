---
api_specs:
- filename: impact-radius-brand-account-v14.yml
  format: yaml
  label: impact.com Brand API
  slug: impactcom-brand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impact-radius/refs/heads/main/openapi/impact-radius-brand-account-v14.yml
- filename: impact-radius-partner-account-v15.yml
  format: yaml
  label: impact.com Partner API
  slug: impactcom-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impact-radius/refs/heads/main/openapi/impact-radius-partner-account-v15.yml
- filename: impact-radius-agency-advertisers-v3.yml
  format: yaml
  label: impact.com Agency API
  slug: impactcom-agency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impact-radius/refs/heads/main/openapi/impact-radius-agency-advertisers-v3.yml
- filename: impact-radius-brand-advocate-account-v13.yml
  format: yaml
  label: impact.com Advocate API
  slug: impactcom-advocate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impact-radius/refs/heads/main/openapi/impact-radius-brand-advocate-account-v13.yml
certifications:
- SOC 1 Type II
- ISO/IEC 27001:2022
- PCI-DSS Level 4
description: impact.com does not run a dedicated trust-center portal (trust.impact.com resolves to the marketing homepage, not a trust page), but it publishes a named security-and-privacy page that lists third-party certifications, compliance processes and security controls. That page is the trust surface of record.
kind: trust-center
layout: security
name: Impact Radius Trust Center
name_suffix: Trust Center
overview: Impact Radius maintains a public trust center documenting SOC 1 Type II, ISO/IEC 27001:2022, and PCI-DSS Level 4 compliance.
provider_name: Impact Radius
provider_slug: impact-radius
slug: impact-radius-trust-center
source_filename: impact-radius-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://impact.com/security-and-privacy/\ndocs:\n- https://impact.com/security-and-privacy/\n- https://impact.responsibledisclosure.com/hc/en-us\ndescription: >-\n  impact.com does not run a dedicated trust-center portal (trust.impact.com resolves to the\n  marketing homepage, not a trust page), but it publishes a named security-and-privacy page that\n  lists third-party certifications, compliance processes and security controls. That page is the\n  trust surface of record.\nportal:\n  url: https://impact.com/security-and-privacy/\n  dedicated_trust_center: false\n  evidence:\n  - url: https://trust.impact.com/\n    status: 200\n    note: >-\n      Returns the impact.com marketing homepage (\"One platform. All partnerships.\"), not a trust\n      center. Recorded as a soft hit, i.e. not a trust document.\n  - url: https://impact.com/security-and-privacy/\n    status: 200\ncertifications:\n- name: SOC 1 Type II\n  scope: Internal\
  \ controls over financial reporting\n  status: certified\n  report_available: not stated\n  source: https://impact.com/security-and-privacy/\n- name: ISO/IEC 27001:2022\n  scope: Information security management system\n  status: certified\n  report_available: not stated\n  source: https://impact.com/security-and-privacy/\n- name: PCI-DSS Level 4\n  scope: Payment card data as a Level 4 Merchant\n  status: certified\n  maintenance: Annual SAQ completion\n  source: https://impact.com/security-and-privacy/\nregulatory:\n- name: GDPR\n  posture: >-\n    States compliant processing, data minimisation on a stated legal basis, no sale of personal\n    data, sharing limited to essential sub-processors, and full data-subject rights (access,\n    rectification, erasure, objection) via compliance@impact.com.\n  contact: compliance@impact.com\n  source: https://impact.com/security-and-privacy/\ncompliance_processes:\n- Consent and opt-out management with customizable forms and participant-controlled\
  \ unsubscribe\n- Right to be forgotten — deletion requests propagate to sub-processors, raised through the support portal\n- Data portability — users can access and view all information associated with their profile\nsecurity_controls:\n- name: Recurring penetration testing\n  detail: >-\n    Independent third-party penetration testing of web applications, mobile apps (Android/iOS)\n    and the underlying APIs.\n- name: Data encryption at rest\n- name: Application security\n- name: Data networking and security\n- name: Restricted access and authorization\n- name: Company security\nnot_claimed:\n  note: >-\n    Recorded explicitly so no reader infers them: no SOC 2 report, no HIPAA, no FedRAMP and no\n    ISO 27017/27018 claim appears on the published page, and no certification report is offered\n    for download or under NDA request.\nvulnerability_disclosure:\n  ref: security/impact-radius-vulnerability-disclosure.yml\n  program: https://impact.responsibledisclosure.com/hc/en-us\nnotes:\
  \ >-\n  Certification names, scopes and maintenance language captured verbatim from the provider's own\n  page. Nothing was inferred from the absence of a trust portal.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/impact-radius/refs/heads/main/security/impact-radius-trust-center.yml
summary_line: SOC 1 Type II, ISO/IEC 27001:2022, PCI-DSS Level 4
tags:
- Company
- Partnership Management
- Affiliate Marketing
- Influencer Marketing
- Referral Marketing
- Attribution
- MarTech
- Advocate
- Creator Economy
- E-Commerce
trust_url: ''
---
