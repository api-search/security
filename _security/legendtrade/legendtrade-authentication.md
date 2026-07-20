---
api_key_in: []
api_specs:
- filename: legendtrade-info-openapi.yml
  format: yaml
  label: Legend Info API
  slug: info
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/legendtrade/refs/heads/main/openapi/legendtrade-info-openapi.yml
- filename: legendtrade-ws-asyncapi.yml
  format: yaml
  label: Legend WebSocket API
  slug: websocket
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/legendtrade/refs/heads/main/asyncapi/legendtrade-ws-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Legendtrade Authentication
name_suffix: Authentication
oauth_flows: []
overview: LegendTrade secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LegendTrade
provider_slug: legendtrade
scheme_count: 1
schemes:
- description: The `/wallets/*` endpoints are authenticated — unauthenticated requests return `401 {"error":"Unauthorized"}`. Legend does not publish the credential format for this operator surface; `bearer` is recorded as the observed-unauthenticated default and is NOT a documented provider claim.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/legendtrade-info-openapi.yml
  type: http
slug: legendtrade-authentication
source_filename: legendtrade-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/legendtrade-info-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: The `/wallets/*` endpoints are authenticated — unauthenticated requests return\n    `401 {\"error\":\"Unauthorized\"}`. Legend does not publish the credential format for this operator\n    surface; `bearer` is recorded as the observed-unauthenticated default and is NOT a documented\n    provider claim.\n  sources:\n  - openapi/legendtrade-info-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/legendtrade/refs/heads/main/authentication/legendtrade-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Defi
- Trading
- Cryptocurrency
- Perpetual Futures
- Social Trading
- Copy Trading
- Market Data
- Hyperliquid
- WebSocket
---
