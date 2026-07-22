---
api_key_in:
- header
api_specs:
- filename: origin-airbrush-openapi-original.yml
  format: yaml
  label: Origin Trades API (Airbrush v3)
  slug: origin-trades-api-airbrush-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origin/refs/heads/main/openapi/origin-airbrush-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Origin Authentication
name_suffix: Authentication
oauth_flows: []
overview: Origin secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Origin
provider_slug: origin
scheme_count: 1
schemes:
- description: 'Unique API key used for authentication, provided by Origin. Scopes the response to the trades the key has been granted access to. Invalid keys return HTTP 403 with a {"detail": "Invalid API Key"} body.

    '
  in: header
  name: API-Key
  parameter_name: API-Key
  sources:
  - openapi/origin-airbrush-openapi-original.yml
  type: apiKey
slug: origin-authentication
source_filename: origin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/origin-airbrush-openapi-original.yml\ndocs: https://airbrush.originmarkets.com/v3/\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nnotes: >\n  The Origin Trades API (Airbrush v3) authenticates with a single API key passed in the\n  API-Key request header, issued by Origin. The Swagger 2.0 document models this as a\n  header parameter rather than a declared securityDefinitions scheme, so the mechanical\n  deriver reports no formal scheme; the auth model below is captured from the documented\n  request header and the per-operation 403 \"Invalid API Key\" response. If the key is\n  omitted the API returns the interactive documentation page instead of data.\nschemes:\n- name: API-Key\n  type: apiKey\n  in: header\n  parameter_name: API-Key\n  description: >\n    Unique API key used for authentication, provided by Origin. Scopes the response to\n    the trades the key has been granted access to.\
  \ Invalid keys return HTTP 403 with a\n    {\"detail\": \"Invalid API Key\"} body.\n  sources: [openapi/origin-airbrush-openapi-original.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/origin/refs/heads/main/authentication/origin-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Financial Services
- Capital Markets
- Bond Issuance
- Debt Capital Markets
- Fixed Income
- Post-Trade
- ISO 20022
- FinTech
- Straight-Through Processing
---
