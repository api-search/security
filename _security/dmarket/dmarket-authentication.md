---
api_key_in:
- header
api_specs:
- filename: dmarket-trading-openapi.yml
  format: yaml
  label: DMarket Trading API
  slug: dmarket-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dmarket/refs/heads/main/openapi/dmarket-trading-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Dmarket Authentication
name_suffix: Authentication
oauth_flows: []
overview: DMarket secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DMarket
provider_slug: dmarket
scheme_count: 3
schemes:
- description: Public API key (lowercase hex). Generate it in your DMarket account settings. See https://dmarket.com/faq#tradingAPI.
  in: header
  name: ApiKey
  parameter: X-Api-Key
  sources:
  - openapi/dmarket-trading-openapi.yml
  type: apiKey
- description: Unix timestamp in seconds at signing time (e.g. 1605619994). Must be within 2 minutes of server time.
  in: header
  name: SignDate
  parameter: X-Sign-Date
  sources:
  - openapi/dmarket-trading-openapi.yml
  type: apiKey
- description: 'Ed25519 request signature prefixed with `dmar ed25519 `. Sign the concatenation of HTTP method + path (including query string) + body + X-Sign-Date with your secret key, then hex-encode the 64-byte Ed25519 signature. Reference clients (Go, Python, JS, PHP): https://github.com/dmarket/dm-trading-tools.'
  in: header
  name: RequestSign
  parameter: X-Request-Sign
  sources:
  - openapi/dmarket-trading-openapi.yml
  type: apiKey
slug: dmarket-authentication
source_filename: dmarket-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/dmarket-trading-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: Public API key (lowercase hex). Generate it in your DMarket account settings.\n    See https://dmarket.com/faq#tradingAPI.\n  sources:\n  - openapi/dmarket-trading-openapi.yml\n- name: SignDate\n  type: apiKey\n  in: header\n  parameter: X-Sign-Date\n  description: Unix timestamp in seconds at signing time (e.g. 1605619994). Must be within 2\n    minutes of server time.\n  sources:\n  - openapi/dmarket-trading-openapi.yml\n- name: RequestSign\n  type: apiKey\n  in: header\n  parameter: X-Request-Sign\n  description: 'Ed25519 request signature prefixed with `dmar ed25519 `. Sign the concatenation\n    of HTTP method + path (including query string) + body + X-Sign-Date with your secret key,\n    then hex-encode the 64-byte Ed25519 signature.\
  \ Reference clients (Go, Python, JS, PHP):\n    https://github.com/dmarket/dm-trading-tools.'\n  sources:\n  - openapi/dmarket-trading-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dmarket/refs/heads/main/authentication/dmarket-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Crypto
- Gaming
- Marketplace
- Trading
- Skins
- In-Game Items
- Blockchain
---
