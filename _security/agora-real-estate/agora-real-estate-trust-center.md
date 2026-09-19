---
api_specs:
- filename: agora-real-estate-agora-content-api-openapi.yml
  format: yaml
  label: Agora Real Estate Agora Content API
  slug: agora-real-estate-agora-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-real-estate/refs/heads/main/openapi/agora-real-estate-agora-content-api-openapi.yml
- filename: agora-real-estate-wordpress-content-api-openapi.yml
  format: yaml
  label: Agora Real Estate WordPress Content API
  slug: agora-real-estate-wordpress-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-real-estate/refs/heads/main/openapi/agora-real-estate-wordpress-content-api-openapi.yml
- filename: agora-real-estate-o-embed-api-openapi.yml
  format: yaml
  label: Agora Real Estate o Embed API
  slug: agora-real-estate-o-embed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora-real-estate/refs/heads/main/openapi/agora-real-estate-o-embed-api-openapi.yml
certification_count: 4
certifications:
- SOC 2 Type II
- SOC 1
- ISO 27001:2022
- GDPR
description: ''
kind: trust-center
layout: security
name: Agora Real Estate Trust Center
name_suffix: Trust Center
overview: Agora Real Estate maintains a public trust center documenting SOC 2 Type II, SOC 1, ISO 27001:2022, and GDPR compliance.
provider_name: Agora Real Estate
provider_slug: agora-real-estate
slug: agora-real-estate-trust-center
source_filename: agora-real-estate-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: >-\n  https://trust.agorareal.com/ and its own public data endpoint\n  https://api.scytale.ai/views/trust-center/public/page-data (HTTP 200, requested with the trust\n  center's Origin), plus https://agorareal.com/security-and-privacy/ (HTTP 200), 2026-09-12.\nurl: https://trust.agorareal.com/\nplatform: Scytale\nplatform_note: >-\n  The trust center is a Scytale-hosted single-page app on Agora's own domain. The page itself renders\n  client-side, so the certification list was read from the public page-data document the app fetches,\n  not asserted from the HTML shell.\nsummary: >-\n  Agora publishes a trust center listing four compliance frameworks, all marked fully implemented,\n  and describes the controls behind them on its own security page. Document downloads (SOC reports,\n  policies) are gated behind a \"Request Access\" form; no policy or report file is public.\ncertifications:\n- name: SOC 2 Type II\n  id: soc2-type2\n\
  \  status: fully-implemented\n  source: trust-center\n- name: SOC 1\n  id: soc1\n  status: fully-implemented\n  source: trust-center\n- name: ISO 27001:2022\n  id: iso27001-2022\n  status: fully-implemented\n  source: trust-center\n- name: GDPR\n  id: gdpr-2024\n  status: fully-implemented\n  source: trust-center\ncontrols_published:\n- Periodic external audits, penetration testing and vulnerability scanning\n- WAF firewall and two-factor authentication\n- 256-bit AES at rest and TLS in transit\n- Automatic database and S3 backup with system redundancy\n- Subprocessor register — 26 vendors listed with name, purpose and processing locations\ndocuments_public: false\ndocuments_note: >-\n  reportFiles and policies are empty in the public payload and the trust center exposes a\n  \"Request Access\" dialog (full name, company, email) for restricted files — certifications are\n  named publicly, the evidence behind them is not.\nevidence:\n- url: https://trust.agorareal.com/\n  status: 200\n\
  - url: https://api.scytale.ai/views/trust-center/public/page-data\n  status: 200\n- url: https://agorareal.com/security-and-privacy/\n  status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agora-real-estate/refs/heads/main/security/agora-real-estate-trust-center.yml
summary_line: SOC 2 Type II, SOC 1, ISO 27001:2022, GDPR
tags:
- Real-Estate
- Investment Management
- Private Equity
- Fund Administration
- Investor Relations
- Capital Raising
- Syndication
- Fund Accounting
- Investor Portal
- CRM
- Payments
- Content Management
- Software-as-a-Service
trust_url: https://trust.agorareal.com/
---
