---
api_key_in:
- header
api_specs:
- filename: breeze-openapi-original.json
  format: json
  label: Breeze API
  slug: breeze-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze/refs/heads/main/openapi/breeze-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Breeze Authentication
name_suffix: Authentication
oauth_flows: []
overview: Breeze secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Breeze
provider_slug: breeze
scheme_count: 2
schemes:
- in: header
  name: api_key
  parameter: x-api-key
  sources:
  - openapi/breeze-openapi-original.json
  type: apiKey
- bearerFormat: JWT
  name: bearer_auth
  scheme: bearer
  sources:
  - openapi/breeze-openapi-original.json
  type: http
slug: breeze-authentication
source_filename: breeze-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/breeze-openapi-original.json\ndocs: https://docs.breeze.baby/get-your-api-key/instruction\nnotes: >-\n  Integration endpoints authenticate with an API key in the x-api-key header\n  (generated in the Breeze Customer Portal, portal.breeze.baby). Organization and\n  admin endpoints use a JWT bearer token. The x402 Agent Kit path is keyless,\n  gated by USDC micropayments instead.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/breeze-openapi-original.json\n- name: bearer_auth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/breeze-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/breeze/refs/heads/main/authentication/breeze-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Crypto Web3
- Solana
- Yield
- DeFi
- Payments
- Blockchain
- API
- AI Agents
---
