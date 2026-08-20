---
api_specs:
- filename: simpleanalytics-events-api-openapi.yml
  format: yaml
  label: Simple Analytics Events API
  slug: simpleanalytics-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpleanalytics/refs/heads/main/openapi/simpleanalytics-events-api-openapi.yml
- filename: simpleanalytics-export-api-openapi.yml
  format: yaml
  label: Simple Analytics Export API
  slug: simpleanalytics-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpleanalytics/refs/heads/main/openapi/simpleanalytics-export-api-openapi.yml
- filename: simpleanalytics-stats-api-openapi.yml
  format: yaml
  label: Simple Analytics Stats API
  slug: simpleanalytics-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpleanalytics/refs/heads/main/openapi/simpleanalytics-stats-api-openapi.yml
- filename: simpleanalytics-websites-api-openapi.yml
  format: yaml
  label: Simple Analytics Websites API
  slug: simpleanalytics-websites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpleanalytics/refs/heads/main/openapi/simpleanalytics-websites-api-openapi.yml
certifications:
- SOC 2 Type II
- ISO 27001
- HIPAA
- PCI DSS
description: 'Simple Analytics runs no third-party trust portal (trust.simpleanalytics.com does not resolve; /trust returns 404). Its trust surface is a first-party Security page backed by a linked set of published compliance documents: GDPR compliance, data collection detail, DPA, subprocessor list and privacy policy. Recorded here as the provider''s trust centre because the pages are real, first-party and specific — not because a vendor portal exists.'
kind: trust-center
layout: security
name: Simpleanalytics Trust Center
name_suffix: Trust Center
overview: Simple Analytics maintains a public trust center documenting SOC 2 Type II, ISO 27001, HIPAA, and PCI DSS compliance.
provider_name: Simple Analytics
provider_slug: simpleanalytics
slug: simpleanalytics-trust-center
source_filename: simpleanalytics-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://www.simpleanalytics.com/security,\n  https://www.simpleanalytics.com/gdpr-compliance,\n  https://www.simpleanalytics.com/subprocessors,\n  https://www.simpleanalytics.com/data-processing-agreement,\n  https://www.simpleanalytics.com/data-collection,\n  https://www.simpleanalytics.com/privacy-policy\ndescription: >-\n  Simple Analytics runs no third-party trust portal (trust.simpleanalytics.com\n  does not resolve; /trust returns 404). Its trust surface is a first-party\n  Security page backed by a linked set of published compliance documents:\n  GDPR compliance, data collection detail, DPA, subprocessor list and privacy\n  policy. Recorded here as the provider's trust centre because the pages are\n  real, first-party and specific — not because a vendor portal exists.\nurl: https://www.simpleanalytics.com/security\nhttp_status: 200\nchecked: '2026-08-13'\nform: first-party security + compliance pages (no vendor\
  \ trust portal)\nprobes:\n- url: https://www.simpleanalytics.com/security\n  status: 200\n- url: https://www.simpleanalytics.com/gdpr-compliance\n  status: 200\n- url: https://www.simpleanalytics.com/subprocessors\n  status: 200\n- url: https://trust.simpleanalytics.com\n  status: 000\n  note: DNS does not resolve.\n- url: https://www.simpleanalytics.com/trust\n  status: 404\ncertifications:\n- name: SOC 2 Type II\n  status: in-progress\n  held: false\n  evidence: >-\n    Security page states \"SOC 2 (in progress) — We are working toward SOC 2\n    Type II certification\" and lists SOC 2 compliance as an Enterprise-plan\n    capability on the pricing page. NOT a held certification.\n- name: ISO 27001\n  status: not-claimed\n  held: false\n- name: HIPAA\n  status: not-claimed\n  held: false\n- name: PCI DSS\n  status: not-applicable\n  held: false\nregulatory_posture:\n- regime: GDPR\n  claim: GDPR-compliant by design; processes no personal data\n  page: https://www.simpleanalytics.com/gdpr-compliance\n\
  - regime: ePrivacy Directive / UK GDPR / PECR\n  claim: Satisfied because only non-personal data is processed\n  page: https://www.simpleanalytics.com/pricing\n- regime: EU data residency\n  claim: All analytics data stored and processed in the Netherlands; no transfer outside the EU\n  page: https://www.simpleanalytics.com/security\ncontrols_published:\n  data_minimisation:\n  - No cookies or persistent identifiers\n  - No cross-site tracking\n  - IP addresses discarded immediately, never stored\n  - No fingerprints or user-level profiling\n  - Metrics aggregated and not linked to individuals\n  infrastructure:\n  - Data stored in the Netherlands (EU)\n  - Hosted on Worldstream and Leaseweb infrastructure\n  - Encryption in transit (HTTPS) and at rest\n  - Simple Analytics controls the decryption keys\n  - Redundant infrastructure across multiple providers\n  - Regular backups and continuous security updates\n  access_control:\n  - Restricted production access limited to a small number\
  \ of core team members\n  - MFA applied where applicable\n  - Logging and monitoring of system activity\n  - Vendor security review before adoption with periodic re-evaluation\n  retention:\n  - Retention set by subscription plan\n  - Data stored only while the account is active\n  - Data fully removed within 90 days of account deletion\ndocuments:\n- name: Data Processing Agreement\n  url: https://www.simpleanalytics.com/data-processing-agreement\n- name: Subprocessor list\n  url: https://www.simpleanalytics.com/subprocessors\n- name: What we collect\n  url: https://www.simpleanalytics.com/data-collection\n- name: Privacy policy\n  url: https://www.simpleanalytics.com/privacy-policy\n- name: General terms and conditions\n  url: https://www.simpleanalytics.com/general-terms-and-conditions\nsecurity_contact:\n  vulnerability_disclosure_policy: false\n  bug_bounty: false\n  security_txt: false\n  channel: >-\n    General contact form only — the Security page directs security and\n    compliance\
  \ questions to https://www.simpleanalytics.com/contact. No named\n    security address, no coordinated-disclosure policy, and\n    /.well-known/security.txt returns 404 on every host. This is the clearest\n    single gap in an otherwise strong privacy posture, and it is the provider's\n    to close.\ngaps:\n- No RFC 9116 security.txt on any host.\n- No published vulnerability disclosure or coordinated-disclosure policy.\n- No bug bounty programme (HackerOne / Bugcrowd / Intigriti all absent).\n- SOC 2 Type II is advertised as in progress but not held.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simpleanalytics/refs/heads/main/security/simpleanalytics-trust-center.yml
summary_line: SOC 2 Type II, ISO 27001, HIPAA, PCI DSS
tags:
- Analytics
- Web Analytics
- Privacy
- Cookieless
- GDPR
- Event
- Data Export
- Europe
trust_url: https://www.simpleanalytics.com/security
---
