---
api_key_in:
- header
api_specs:
- filename: doppel-alerts-api-openapi.yml
  format: yaml
  label: Doppel alerts API
  slug: doppel-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doppel/refs/heads/main/openapi/doppel-alerts-api-openapi.yml
- filename: doppel-brands-api-openapi.yml
  format: yaml
  label: Doppel brands API
  slug: doppel-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doppel/refs/heads/main/openapi/doppel-brands-api-openapi.yml
- filename: doppel-hrm-api-openapi.yml
  format: yaml
  label: Doppel hrm API
  slug: doppel-hrm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doppel/refs/heads/main/openapi/doppel-hrm-api-openapi.yml
- filename: doppel-phishing-simulation-api-openapi.yml
  format: yaml
  label: Doppel phishing-simulation API
  slug: doppel-phishing-simulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doppel/refs/heads/main/openapi/doppel-phishing-simulation-api-openapi.yml
- filename: doppel-protected-assets-api-openapi.yml
  format: yaml
  label: Doppel protected-assets API
  slug: doppel-protected-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doppel/refs/heads/main/openapi/doppel-protected-assets-api-openapi.yml
- filename: doppel-reports-api-openapi.yml
  format: yaml
  label: Doppel reports API
  slug: doppel-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doppel/refs/heads/main/openapi/doppel-reports-api-openapi.yml
- filename: doppel-scan-api-openapi.yml
  format: yaml
  label: Doppel scan API
  slug: doppel-scan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doppel/refs/heads/main/openapi/doppel-scan-api-openapi.yml
- filename: doppel-iocs-api-openapi.yml
  format: yaml
  label: Doppel Iocs API
  slug: doppel-iocs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doppel/refs/heads/main/openapi/doppel-iocs-api-openapi.yml
- filename: doppel-reports-deprecated-api-openapi.yml
  format: yaml
  label: Doppel reports (deprecated) API
  slug: doppel-reports-deprecated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doppel/refs/heads/main/openapi/doppel-reports-deprecated-api-openapi.yml
- filename: doppel-sms-responses-api-openapi.yml
  format: yaml
  label: Doppel Sms Responses API
  slug: doppel-sms-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doppel/refs/heads/main/openapi/doppel-sms-responses-api-openapi.yml
- filename: doppel-urls-api-openapi.yml
  format: yaml
  label: Doppel URLS API
  slug: doppel-urls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doppel/refs/heads/main/openapi/doppel-urls-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Doppel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Doppel secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Doppel
provider_slug: doppel
scheme_count: 2
schemes:
- description: API key from Doppel Vision API settings. Required for gateway authentication and quota.
  in: header
  name: api_key
  parameter: x-api-key
  sources:
  - openapi/doppel-openapi-original.yml
  type: apiKey
- description: User API key from Doppel Vision API settings. Required together with x-api-key for authenticated requests.
  in: header
  name: user_api_key
  parameter: x-user-api-key
  sources:
  - openapi/doppel-openapi-original.yml
  type: apiKey
slug: doppel-authentication
source_filename: doppel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/doppel-openapi-original.yml\ndocs: https://doppel.readme.io/docs/authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  notes: >-\n    Doppel V1 authenticates with static API keys passed as request headers. User-specific\n    (recommended): send both x-api-key (org key) and x-user-api-key (per-user, self-service,\n    self-rotatable, RBAC-scoped). Organization-wide: send x-api-key only. No OAuth2/OIDC surface.\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key from Doppel Vision API settings. Required for gateway authentication\n    and quota.\n  sources:\n  - openapi/doppel-openapi-original.yml\n- name: user_api_key\n  type: apiKey\n  in: header\n  parameter: x-user-api-key\n  description: User API key from Doppel Vision API settings. Required together with x-api-key\n    for authenticated requests.\n  sources:\n  - openapi/doppel-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doppel/refs/heads/main/authentication/doppel-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Security
- Cybersecurity
- Digital Risk Protection
- Social Engineering Defense
- Brand Protection
- Anti-Phishing
- Threat Intelligence
- Human Risk Management
- Takedowns
---
