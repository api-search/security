---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Alt Bank Authentication
name_suffix: Authentication
oauth_flows: []
overview: Alt Bank secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Alt Bank
provider_slug: alt-bank
scheme_count: 1
schemes:
- description: A 64-character alphanumeric token that uniquely identifies the partner and is sent on the X-Partner-Auth request header for every GUARD API call.
  format: 64-character alphanumeric string
  in: header
  name: X-Partner-Auth
  parameter_name: X-Partner-Auth
  sources:
  - https://developers.altbank.ai/docs/guard-api
  type: apiKey
slug: alt-bank-authentication
source_filename: alt-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://developers.altbank.ai/docs/guard-api\ndocs: https://developers.altbank.ai/docs/guard-api\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    alt.bank authenticates partners with a static per-partner API token, not\n    OAuth. There is no documented OAuth2/OIDC scope surface, so no scopes/\n    artifact is emitted.\nschemes:\n- name: X-Partner-Auth\n  type: apiKey\n  in: header\n  parameter_name: X-Partner-Auth\n  description: >-\n    A 64-character alphanumeric token that uniquely identifies the partner and\n    is sent on the X-Partner-Auth request header for every GUARD API call.\n  format: 64-character alphanumeric string\n  sources: [https://developers.altbank.ai/docs/guard-api]\nnetwork_controls:\n- type: ip-allowlist\n  description: >-\n    Partners must register the list of source IP addresses from which API\n    requests originate; alt.bank locks API communication down\
  \ to those\n    predefined addresses in addition to token auth.\n  sources: [https://developers.altbank.ai/docs/guard-api]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alt-bank/refs/heads/main/authentication/alt-bank-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Fintech
- Banking
- Credit
- Underwriting
- Credit Cards
- Payments
- KYC
- Risk
- Brazil
- Financial Inclusion
- Banking as a Service
---
