---
api_key_in: []
api_specs:
- filename: btc-war-live-market-data-api-market-data-openapi.yml
  format: yaml
  label: BTC War Live Market Data API
  slug: btc-war-live-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/btc-war-live-market-data-api/refs/heads/main/openapi/btc-war-live-market-data-api-market-data-openapi.yml
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: Btc War Live Market Data Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: BTC War Live Market Data API secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: BTC War Live Market Data API
provider_slug: btc-war-live-market-data-api
scheme_count: 0
schemes: []
slug: btc-war-live-market-data-api-authentication
source_filename: btc-war-live-market-data-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: searched\nsource: https://btcwar.net/api/openapi.json\ndocs: https://btcwar.net/btc-price\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\n  authentication_required: false\n  note: >-\n    The API declares an empty root-level `security: []` and repeats `security: []` on every operation, which is an\n    explicit OpenAPI 3.1 statement that no security scheme applies. No securitySchemes are defined because none exist.\nschemes: []\npublic_access:\n  keyless: true\n  account_required: false\n  registration_required: false\n  payment_required: false\n  cors: \"access-control-allow-origin: *\"\n  evidence:\n    - url: https://btcwar.net/api/market-snapshot/v1.json\n      http_status: 200\n      note: Anonymous GET returned a complete 200 response with no credential of any kind.\n    - url: https://btcwar.net/mcp\n      http_status: 200\n      note: MCP initialize + tools/list answered anonymously; /.well-known/mcp.json declares authentication.required\
  \ false.\n    - url: https://btcwar.net/llms.txt\n      http_status: 200\n      note: \"Publisher statement: API access is USD 0 with no account, no API key, no registration and no payment required.\"\ngaps:\n  - No OAuth surface exists, so scopes/ is not applicable to this provider.\n  - No per-caller identity means no per-caller rate limit, quota or usage attribution is possible.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/btc-war-live-market-data-api/refs/heads/main/authentication/btc-war-live-market-data-api-authentication.yml
summary_line: none · 0 schemes
tags:
- finance
- cryptocurrency
- market-data
- bitcoin
- crypto-price
- binance-spot
- order-flow
- market-depth
- json-ld
- schema.org
- openapi
- mcp
- read-only
- no-authentication
- agent-native
- arazzo
- json-schema
- agent-skill
---
