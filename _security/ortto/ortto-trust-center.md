---
api_specs:
- filename: ortto-accounts-api-openapi.yml
  format: yaml
  label: Ortto Accounts API
  slug: ortto-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/openapi/ortto-accounts-api-openapi.yml
- filename: ortto-activities-api-openapi.yml
  format: yaml
  label: Ortto Activities API
  slug: ortto-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/openapi/ortto-activities-api-openapi.yml
- filename: ortto-campaigns-api-openapi.yml
  format: yaml
  label: Ortto Campaigns API
  slug: ortto-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/openapi/ortto-campaigns-api-openapi.yml
- filename: ortto-people-api-openapi.yml
  format: yaml
  label: Ortto People API
  slug: ortto-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/openapi/ortto-people-api-openapi.yml
- filename: ortto-tags-api-openapi.yml
  format: yaml
  label: Ortto Tags API
  slug: ortto-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/openapi/ortto-tags-api-openapi.yml
- filename: ortto-transactional-api-openapi.yml
  format: yaml
  label: Ortto Transactional API
  slug: ortto-transactional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/openapi/ortto-transactional-api-openapi.yml
certifications:
- SOC 2
- ISO 27001
- GDPR
- CCPA
- EU-US Data Privacy Framework
description: 'Ortto''s security and privacy page is its trust surface. It names four compliance programs in a single sentence and lists the platform controls behind them, but it is a marketing page rather than a trust portal: there is no self-service document request flow, no downloadable SOC 2 report, no sub-processor list on the page, and no third-party trust-center host (Vanta, Drata, SafeBase). Audit reports are "available on request".'
kind: trust-center
layout: security
name: Ortto Trust Center
name_suffix: Trust Center
overview: Ortto maintains a public trust center documenting SOC 2, ISO 27001, GDPR, CCPA, and EU-US Data Privacy Framework compliance.
provider_name: Ortto
provider_slug: ortto
slug: ortto-trust-center
source_filename: ortto-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://ortto.com/security-privacy/\ndescription: >-\n  Ortto's security and privacy page is its trust surface. It names four\n  compliance programs in a single sentence and lists the platform controls\n  behind them, but it is a marketing page rather than a trust portal: there is\n  no self-service document request flow, no downloadable SOC 2 report, no\n  sub-processor list on the page, and no third-party trust-center host (Vanta,\n  Drata, SafeBase). Audit reports are \"available on request\".\ntrust_center:\n  url: https://ortto.com/security-privacy/\n  status: 200\n  checked: '2026-08-13'\n  platform: first-party page\n  self_service_documents: false\n  report_access: on request\n  quote: Our latest audit reports are available on request\ncertifications:\n- name: SOC 2\n  claimed: true\n  self_asserted: true\n  evidence: '\"We are GDPR, CCPA, ISO27001^ and SOC2 compliant\"'\n  report_public: false\n- name: ISO 27001\n\
  \  claimed: true\n  self_asserted: true\n  evidence: Named in the same statement, carrying a footnote marker.\n  report_public: false\n- name: GDPR\n  claimed: true\n  evidence: >-\n    Named in the same statement; dedicated page at https://ortto.com/gdpr/\n    (HTTP 200).\n- name: CCPA\n  claimed: true\n  evidence: Named in the same statement.\n- name: EU-US Data Privacy Framework\n  claimed: true\n  evidence: 'Dedicated page at https://ortto.com/dpf/ (HTTP 200).'\nmemberships:\n- name: M3AAWG\n  description: >-\n    Messaging, Malware and Mobile Anti-Abuse Working Group; Ortto describes\n    itself as \"a member of anti-abuse organization M3AAWG\" and announced the\n    membership on its blog on 2024-12-20.\ncontrols:\n- two-factor authentication\n- user roles and permissions\n- audit logs\n- single sign-on (SSO) and Okta support\n- multi-region data hosting (EU, USA, Australia, Asia)\n- cookie-tracking opt-in for GDPR\n- Google reCAPTCHA on forms\n- incident reporting with live status\
  \ updates\ndata_residency:\n  regions:\n  - EU\n  - USA\n  - Australia\n  - Asia\n  api_endpoints:\n  - https://api.ap3api.com/v1\n  - https://api.eu.ap3api.com/v1\n  - https://api.au.ap3api.com/v1\npolicies:\n  privacy: https://ortto.com/privacy/\n  terms: https://ortto.com/terms/\n  gdpr: https://ortto.com/gdpr/\n  dpf: https://ortto.com/dpf/\n  responsible_disclosure: https://ortto.com/policies/ResponsibleDisclosure.pdf\n  security_txt: https://ortto.com/.well-known/security.txt\nsee_also:\n- security/ortto-vulnerability-disclosure.yml\n- conformance/ortto-conformance.yml\nsummary:\n  certifications_named: 5\n  reports_downloadable: false\n  third_party_trust_portal: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ortto/refs/heads/main/security/ortto-trust-center.yml
summary_line: SOC 2, ISO 27001, GDPR, CCPA, EU-US Data Privacy Framework
tags:
- Marketing Automation
- CDP
- Customer Data Platform
- Analytics
- Email
- SMS
- Transactional Email
- Webhooks
- MCP
- Push Notifications
trust_url: ''
---
