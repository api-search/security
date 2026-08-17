---
api_specs:
- filename: lusha-search-api-openapi.yml
  format: yaml
  label: Lusha Search API
  slug: lusha-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-search-api-openapi.yml
- filename: lusha-enrich-api-openapi.yml
  format: yaml
  label: Lusha Enrich API
  slug: lusha-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-enrich-api-openapi.yml
- filename: lusha-search-enrich-api-openapi.yml
  format: yaml
  label: Lusha Search & Enrich API
  slug: lusha-search-enrich-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-search-enrich-api-openapi.yml
- filename: lusha-prospecting-api-openapi.yml
  format: yaml
  label: Lusha Prospecting API
  slug: lusha-prospecting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-prospecting-api-openapi.yml
- filename: lusha-lookalikes-api-openapi.yml
  format: yaml
  label: Lusha Lookalikes API
  slug: lusha-lookalike-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-lookalikes-api-openapi.yml
- filename: lusha-buying-group-api-openapi.yml
  format: yaml
  label: Lusha Buying Group API
  slug: lusha-buying-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-buying-group-api-openapi.yml
- filename: lusha-signals-api-openapi.yml
  format: yaml
  label: Lusha Signals API
  slug: lusha-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-signals-api-openapi.yml
- filename: lusha-website-visits-api-openapi.yml
  format: yaml
  label: Lusha Website Visitors API
  slug: lusha-website-visits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-website-visits-api-openapi.yml
- filename: lusha-filters-api-openapi.yml
  format: yaml
  label: Lusha Filters API
  slug: lusha-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-filters-api-openapi.yml
- filename: lusha-contacts-tables-api-openapi.yml
  format: yaml
  label: Lusha Contacts Tables API
  slug: lusha-contacts-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-contacts-tables-api-openapi.yml
- filename: lusha-companies-tables-api-openapi.yml
  format: yaml
  label: Lusha Companies Tables API
  slug: lusha-companies-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-companies-tables-api-openapi.yml
- filename: lusha-webhooks-api-openapi.yml
  format: yaml
  label: Lusha Webhooks API
  slug: lusha-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-webhooks-api-openapi.yml
- filename: lusha-account-api-openapi.yml
  format: yaml
  label: Lusha Account API
  slug: lusha-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/openapi/lusha-account-api-openapi.yml
certifications:
- SOC 2 Type II
description: Lusha runs a trust centre at https://www.lusha.com/trust-center. The automated probe of that URL returned HTTP 403 (Cloudflare "Just a moment..." interstitial on the marketing host), so the certifications below are read from Lusha's own documentation host, which names the trust centre as the place its compliance documents live and states the SOC 2 Type II certification outright.
kind: trust-center
layout: security
name: Lusha Trust Center
name_suffix: Trust Center
overview: Lusha maintains a public trust center documenting SOC 2 Type II compliance.
provider_name: Lusha
provider_slug: lusha
slug: lusha-trust-center
source_filename: lusha-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nurl: https://www.lusha.com/trust-center\ndescription: >-\n  Lusha runs a trust centre at https://www.lusha.com/trust-center. The automated\n  probe of that URL returned HTTP 403 (Cloudflare \"Just a moment...\" interstitial\n  on the marketing host), so the certifications below are read from Lusha's own\n  documentation host, which names the trust centre as the place its compliance\n  documents live and states the SOC 2 Type II certification outright.\ncertifications:\n- SOC 2 Type II\nregulations:\n- GDPR\ndocuments:\n- name: Security overview\n  availability: public (docs host)\n  url: https://docs.lusha.com/user-guide/security/lusha-security-overview\n- name: Privacy policy\n  availability: public\n  url: https://lusha.com/legal/privacy-notice/\n- name: Sub-processor list\n  availability: public (trust centre)\n- name: SOC 2 Type II report\n  availability: gated\n  gate: Scale plan customers, or accounts with transactions\
  \ exceeding $10,000\n- name: Penetration test report\n  availability: gated\n  gate: NDA required\n  note: findings assessed as very low risk; no separate remediation plan provided\ncontrols_published:\n- Encryption in transit (TLS)\n- Encryption at rest\n- Role-based access control (Admin / Manager / User)\n- SSO via SAML 2.0 (Scale plan) with Okta and custom IdP guides\n- Automatic inactive-session termination and sign-out-of-all-sessions\n- Minimum password strength enforcement\nsecurity_contact: security@lusha.com\nevidence:\n- source: https://docs.lusha.com/user-guide/security/lusha-security-overview\n  http_status: 200\n  keywords: [SOC 2 Type II, GDPR, trust center, penetration test, encryption at rest, RBAC, SAML]\n- source: https://www.lusha.com/trust-center\n  http_status: 403\n  note: Cloudflare bot challenge; page not readable by an automated client\n- source: https://www.lusha.com/.well-known/security.txt\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lusha/refs/heads/main/security/lusha-trust-center.yml
summary_line: SOC 2 Type II
tags:
- Sales Intelligence
- B2B
- Enrichment
- Contact Data
- Prospecting
- Intent
- Signals
- Lookalikes
- Webhooks
- MCP
trust_url: https://www.lusha.com/trust-center
---
