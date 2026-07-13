---
api_key_in:
- header
api_specs:
- filename: complyadvantage-openapi.yml
  format: yaml
  label: ComplyAdvantage Search API
  slug: complyadvantage-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/complyadvantage/refs/heads/main/openapi/complyadvantage-openapi.yml
- filename: complyadvantage-openapi.yml
  format: yaml
  label: ComplyAdvantage Monitored Search API
  slug: complyadvantage-monitored-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/complyadvantage/refs/heads/main/openapi/complyadvantage-openapi.yml
- filename: complyadvantage-openapi.yml
  format: yaml
  label: ComplyAdvantage Case Management API
  slug: complyadvantage-case-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/complyadvantage/refs/heads/main/openapi/complyadvantage-openapi.yml
- filename: complyadvantage-openapi.yml
  format: yaml
  label: ComplyAdvantage Users API
  slug: complyadvantage-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/complyadvantage/refs/heads/main/openapi/complyadvantage-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Complyadvantage Authentication
name_suffix: Authentication
oauth_flows: []
overview: ComplyAdvantage secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ComplyAdvantage
provider_slug: complyadvantage
scheme_count: 1
schemes:
- description: 'API key sent as: Authorization: Token YOUR_API_KEY. Keys are generated in the ComplyAdvantage web platform.'
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/complyadvantage-openapi.yml
  type: apiKey
slug: complyadvantage-authentication
source_filename: complyadvantage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/complyadvantage-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API key sent as: Authorization: Token YOUR_API_KEY. Keys are generated in the\n    ComplyAdvantage web platform.'\n  sources:\n  - openapi/complyadvantage-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/complyadvantage/refs/heads/main/authentication/complyadvantage-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Anti-Money Laundering
- AML
- Fraud Detection
- Sanctions Screening
- Compliance
- PEP Screening
- Adverse Media
- KYC
- Watchlists
- Transaction Monitoring
- Financial Crime
- RegTech
---
