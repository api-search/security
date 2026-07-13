---
api_key_in:
- header
- query
api_specs:
- filename: openapi.yml
  format: yaml
  label: WazirX REST API
  slug: wazirx-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazirx/refs/heads/main/openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Wazirx Authentication
name_suffix: Authentication
oauth_flows: []
overview: WazirX secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: WazirX
provider_slug: wazirx
scheme_count: 2
schemes:
- description: API key required for MARKET_DATA and SIGNED endpoints
  in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/openapi.yml
  type: apiKey
- description: HMAC SHA256 signature of the request parameters using the secret key
  in: query
  name: HmacSignature
  parameter: signature
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: wazirx-authentication
source_filename: wazirx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: API key required for MARKET_DATA and SIGNED endpoints\n  sources:\n  - openapi/openapi.yml\n- name: HmacSignature\n  type: apiKey\n  in: query\n  parameter: signature\n  description: HMAC SHA256 signature of the request parameters using the secret key\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wazirx/refs/heads/main/authentication/wazirx-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Cryptocurrency
- Exchange
- Trading
- INR
- India
- Bitcoin
- WebSocket
- Market Data
---
