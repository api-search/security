---
api_key_in:
- header
- query
api_specs:
- filename: wazirx-websocket-api-openapi.yml
  format: yaml
  label: WazirX WebSocket API
  slug: wazirx-websocket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazirx/refs/heads/main/openapi/wazirx-websocket-api-openapi.yml
- filename: wazirx-account-api-openapi.yml
  format: yaml
  label: WazirX Account API
  slug: wazirx-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazirx/refs/heads/main/openapi/wazirx-account-api-openapi.yml
- filename: wazirx-general-api-openapi.yml
  format: yaml
  label: WazirX General API
  slug: wazirx-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazirx/refs/heads/main/openapi/wazirx-general-api-openapi.yml
- filename: wazirx-market-data-api-openapi.yml
  format: yaml
  label: WazirX Market Data API
  slug: wazirx-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazirx/refs/heads/main/openapi/wazirx-market-data-api-openapi.yml
- filename: wazirx-sub-account-api-openapi.yml
  format: yaml
  label: WazirX Sub-Account API
  slug: wazirx-sub-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazirx/refs/heads/main/openapi/wazirx-sub-account-api-openapi.yml
- filename: wazirx-trading-api-openapi.yml
  format: yaml
  label: WazirX Trading API
  slug: wazirx-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazirx/refs/heads/main/openapi/wazirx-trading-api-openapi.yml
- filename: wazirx-wallet-api-openapi.yml
  format: yaml
  label: WazirX Wallet API
  slug: wazirx-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazirx/refs/heads/main/openapi/wazirx-wallet-api-openapi.yml
- filename: wazirx-websocket-api-openapi.yml
  format: yaml
  label: WazirX WebSocket API
  slug: wazirx-websocket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazirx/refs/heads/main/openapi/wazirx-websocket-api-openapi.yml
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
