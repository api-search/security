---
api_key_in:
- header
api_specs:
- filename: lootrush-openapi-original.json
  format: json
  label: LootRush Partner API
  slug: lootrush-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lootrush/refs/heads/main/openapi/lootrush-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lootrush Authentication
name_suffix: Authentication
oauth_flows: []
overview: LootRush secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: LootRush
provider_slug: lootrush
scheme_count: 2
schemes:
- description: 'API token issued by your LootRush account manager. Sent as `Authorization: Bearer <token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/lootrush-openapi-original.json
  type: http
- description: Integration API key provided by LootRush during Connect registration.
  in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/lootrush-openapi-original.json
  type: apiKey
slug: lootrush-authentication
source_filename: lootrush-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/lootrush-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API token issued by your LootRush account manager. Sent as `Authorization: Bearer\n    <token>`.'\n  sources:\n  - openapi/lootrush-openapi-original.json\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Integration API key provided by LootRush during Connect registration.\n  sources:\n  - openapi/lootrush-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lootrush/refs/heads/main/authentication/lootrush-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Gaming
- Crypto
- Cryptocurrency
- Payments
- Withdrawals
- MCP
- API
---
