---
api_key_in:
- header
api_specs:
- filename: contract.yml
  format: yaml
  label: Phemex Contract Trading API
  slug: phemex-contract-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phemex/refs/heads/main/openapi/contract.yml
- filename: spot.yml
  format: yaml
  label: Phemex Spot Trading API
  slug: phemex-spot-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phemex/refs/heads/main/openapi/spot.yml
- filename: hedged-perpetual.yml
  format: yaml
  label: Phemex Hedged Perpetual API
  slug: phemex-hedged-perpetual-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phemex/refs/heads/main/openapi/hedged-perpetual.yml
- filename: transfer.yml
  format: yaml
  label: Phemex Asset Transfer API
  slug: phemex-asset-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phemex/refs/heads/main/openapi/transfer.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Phemex Authentication
name_suffix: Authentication
oauth_flows: []
overview: Phemex secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Phemex
provider_slug: phemex
scheme_count: 1
schemes:
- description: HMAC SHA256 signed request. Also requires x-phemex-request-expiry and x-phemex-request-signature headers.
  in: header
  name: HmacAuth
  parameter: x-phemex-access-token
  sources:
  - openapi/contract.yml
  - openapi/hedged-perpetual.yml
  - openapi/spot.yml
  - openapi/transfer.yml
  type: apiKey
slug: phemex-authentication
source_filename: phemex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/contract.yml, openapi/hedged-perpetual.yml, openapi/spot.yml, openapi/transfer.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: HmacAuth\n  type: apiKey\n  in: header\n  parameter: x-phemex-access-token\n  description: HMAC SHA256 signed request. Also requires x-phemex-request-expiry and x-phemex-request-signature\n    headers.\n  sources:\n  - openapi/contract.yml\n  - openapi/hedged-perpetual.yml\n  - openapi/spot.yml\n  - openapi/transfer.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phemex/refs/heads/main/authentication/phemex-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cryptocurrency
- Derivatives
- Spot Trading
- Perpetual Contracts
- Futures
- WebSocket
- Market Data
---
