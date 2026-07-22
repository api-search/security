---
api_key_in:
- header
api_specs:
- filename: ondo-finance-gm-openapi-original.json
  format: json
  label: Ondo GM Backend API (Ondo Stocks / Global Markets)
  slug: ondo-gm-backend-api-ondo-stocks-global-markets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ondo-finance/refs/heads/main/openapi/ondo-finance-gm-openapi-original.json
- filename: ondo-finance-perps-openapi-original.json
  format: json
  label: Ondo Perps REST API
  slug: ondo-perps-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ondo-finance/refs/heads/main/openapi/ondo-finance-perps-openapi-original.json
- filename: ondo-finance-perps-ws-openapi-original.json
  format: json
  label: Ondo Perps WebSocket API
  slug: ondo-perps-websocket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ondo-finance/refs/heads/main/openapi/ondo-finance-perps-ws-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ondo Finance Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ondo Finance secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ondo Finance
provider_slug: ondo-finance
scheme_count: 3
schemes:
- in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/ondo-finance-gm-openapi-original.json
  type: apiKey
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/ondo-finance-perps-openapi-original.json
  type: http
- in: header
  name: ApiKeyAuth
  parameter: X-API-KEY-ID
  sources:
  - openapi/ondo-finance-perps-openapi-original.json
  type: apiKey
slug: ondo-finance-authentication
source_filename: ondo-finance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/ondo-finance-gm-openapi-original.json, openapi/ondo-finance-perps-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/ondo-finance-gm-openapi-original.json\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/ondo-finance-perps-openapi-original.json\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY-ID\n  sources:\n  - openapi/ondo-finance-perps-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ondo-finance/refs/heads/main/authentication/ondo-finance-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Crypto
- Tokenization
- Real World Assets
- DeFi
- Stocks
- Trading
- Perpetual Futures
- Market Data
- Blockchain
- Financial Services
---
