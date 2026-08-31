---
api_specs:
- filename: usergems-accounts-api-openapi.yml
  format: yaml
  label: UserGems Accounts API
  slug: usergems-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usergems/refs/heads/main/openapi/usergems-accounts-api-openapi.yml
- filename: usergems-contacts-api-openapi.yml
  format: yaml
  label: UserGems Contacts API
  slug: usergems-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usergems/refs/heads/main/openapi/usergems-contacts-api-openapi.yml
- filename: usergems-privacy-api-openapi.yml
  format: yaml
  label: UserGems Privacy API
  slug: usergems-privacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usergems/refs/heads/main/openapi/usergems-privacy-api-openapi.yml
certifications:
- SOC 2 Type II
- GDPR
- CCPA
- EU AI Act (limited risk)
description: UserGems runs a hosted trust center with a document library available on request, plus a public data-security page. Certifications and frameworks below are read from the trust center's own published highlights and from the data-security page.
kind: trust-center
layout: security
name: Usergems Trust Center
name_suffix: Trust Center
overview: UserGems maintains a public trust center documenting SOC 2 Type II, GDPR, CCPA, and EU AI Act (limited risk) compliance.
provider_name: UserGems
provider_slug: usergems
slug: usergems-trust-center
source_filename: usergems-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nsource: https://trust.usergems.com/\nurl: https://trust.usergems.com/\nalso:\n  - https://www.usergems.com/data-security\n  - https://www.usergems.com/legal-security/security\ndescription: >-\n  UserGems runs a hosted trust center with a document library available on\n  request, plus a public data-security page. Certifications and frameworks below\n  are read from the trust center's own published highlights and from the\n  data-security page.\ncertifications:\n  - SOC 2 Type II\n  - GDPR\n  - CCPA\n  - EU AI Act (limited risk)\nframeworks:\n  - CAIQ v4.0.2 (self-assessment)\n  - CAIQ v4.1.0 (self-assessment)\n  - SIG Core v1.2\ndocument_categories:\n  - Self-assessments (CAIQ, SIG Core)\n  - App Security (Responsible Disclosure, Application Penetration Testing, Bot Detection)\n  - Access Control (access log management, automated account management)\n  - Data Privacy (breach notifications, data into/out of system)\n  -\
  \ Legal (Subprocessors, Certificate of Insurance, Data Processing Agreement)\n  - Endpoint Security (EDR, anti-malware)\n  - AI (AI Overview, AI Policies, Risk Profile, Impact Level)\nsecurity_posture:\n  hosting: AWS (US), with EU data-transfer documentation in the Data Privacy section\n  runtime_protection: CrowdStrike managed 24/7 runtime protection\n  encryption_at_rest: AES-256, with KMS-based protection of secrets\n  encryption_in_transit: TLS + HSTS\n  penetration_testing: independent third party, on major change and at least annually\npublic_pages:\n  - url: https://www.usergems.com/data-security\n    http_status: 200\n    finding: SOC 2 Type 2 Certified, GDPR Compliant, regular penetration testing\n  - url: https://www.usergems.com/gdpr\n    http_status: 200\n  - url: https://www.usergems.com/legal-security/data-processing-addendum\n    http_status: 301\n    finding: redirects to a published DPA PDF\nevidence:\n  - source: https://trust.usergems.com/\n    http_status: 200\n  \
  \  keywords:\n      - SOC 2 Type II\n      - GDPR\n      - CCPA\n      - EU AI Act\n      - CAIQ\n      - SIG Core\n      - trust center\n  - source: https://www.usergems.com/data-security\n    http_status: 200\n    keywords:\n      - SOC 2 Type 2 Certified\n      - GDPR Compliant\n      - penetration testing\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usergems/refs/heads/main/security/usergems-trust-center.yml
summary_line: SOC 2 Type II, GDPR, CCPA, EU AI Act (limited risk)
tags:
- Sales Intelligence
- Outbound
- ABM
- Champion Tracking
- Job Changes
- Buying Signals
- AI Scoring
- Sales Engagement
- CRM
- Revenue Operations
- GTM
- MCP
- AI Agents
trust_url: https://trust.usergems.com/
---
