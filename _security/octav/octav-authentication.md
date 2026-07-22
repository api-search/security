---
api_key_in: []
api_specs:
- filename: octav-openapi-original.json
  format: json
  label: Octav API
  slug: octav-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octav/refs/heads/main/openapi/octav-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Octav Authentication
name_suffix: Authentication
oauth_flows: []
overview: Octav secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Octav
provider_slug: octav
scheme_count: 1
schemes:
- format: 'Authorization: Bearer <API_KEY>'
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/octav-openapi-original.json
  type: http
slug: octav-authentication
source_filename: octav-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/octav-openapi-original.json\ndocs: https://docs.octav.fi/api/authentication\nsummary:\n  types:\n  - http\n  scheme: bearer\n  token: API key issued from the developer portal, sent as a Bearer token\n  key_management: Create/name/rotate keys at https://data.octav.fi (API Keys section); key shown once and cannot be retrieved later\n  best_practices:\n  - store keys in environment variables (OCTAV_API_KEY), never hardcode or commit\n  - rotate keys periodically; use distinct keys per environment (prod/staging/dev/CI)\n  - monitor usage and set alerts in the developer portal\n  test_endpoint: GET /v1/credits (free) to verify authentication at zero cost\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer <API_KEY>'\n  sources:\n  - openapi/octav-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/octav/refs/heads/main/authentication/octav-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Cryptocurrency
- Blockchain
- Portfolio
- DeFi
- Analytics
- Web3
- Financial Data
- Wallet
---
