---
api_key_in: []
api_specs:
- filename: pyth-hermes-openapi-original.json
  format: json
  label: Pyth Hermes (Pyth Core)
  slug: pyth-hermes-pyth-core
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pyth/refs/heads/main/openapi/pyth-hermes-openapi-original.json
- filename: pyth-benchmarks-openapi-original.json
  format: json
  label: Pyth Benchmarks
  slug: pyth-benchmarks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pyth/refs/heads/main/openapi/pyth-benchmarks-openapi-original.json
auth_types:
- none
- http
description: ''
kind: authentication
layout: security
method: searched
name: Pyth Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pyth secures its APIs with none and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Pyth
provider_slug: pyth
scheme_count: 3
schemes:
- applies_to: openapi/pyth-hermes-openapi-original.json
  description: Hermes REST/SSE endpoints are currently public (rate-limited, no auth in the OpenAPI). An API key becomes required 2026-08-18 (see lifecycle/pyth-lifecycle.yml).
  name: HermesPublic
  type: none
- applies_to: openapi/pyth-benchmarks-openapi-original.json
  description: Benchmarks (historical / TradingView shim) endpoints are public; no securityScheme declared.
  name: BenchmarksPublic
  type: none
- applies_to: Pyth Pro (Lazer) WebSocket + authenticated HTTP (History/REST) + MCP price tools
  description: 'API key issued from the Pyth Terminal (https://pythdata.app -> View your API key), passed as `Authorization: Bearer {key}`. In the MCP server it is passed as the `access_token` argument. Provider guidance: never embed the key in browser/frontend apps — proxy through your backend.'
  name: PythProBearer
  scheme: bearer
  type: http
slug: pyth-authentication
source_filename: pyth-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.pyth.network/price-feeds/pro/acquire-api-key, docs.pyth.network/SKILL.md\ndocs: https://docs.pyth.network/price-feeds/pro/acquire-api-key\nsummary:\n  types: [none, http]\n  http_schemes: [bearer]\n  note: >-\n    Read APIs are historically public. Pyth Pro (Lazer) and the MCP/history endpoints use a\n    Bearer API key. The Hermes public price API is scheduled to require a Pyth API key from\n    2026-08-18.\nschemes:\n  - name: HermesPublic\n    type: none\n    applies_to: openapi/pyth-hermes-openapi-original.json\n    description: >-\n      Hermes REST/SSE endpoints are currently public (rate-limited, no auth in the OpenAPI).\n      An API key becomes required 2026-08-18 (see lifecycle/pyth-lifecycle.yml).\n  - name: BenchmarksPublic\n    type: none\n    applies_to: openapi/pyth-benchmarks-openapi-original.json\n    description: Benchmarks (historical / TradingView shim) endpoints are public; no securityScheme\
  \ declared.\n  - name: PythProBearer\n    type: http\n    scheme: bearer\n    applies_to: Pyth Pro (Lazer) WebSocket + authenticated HTTP (History/REST) + MCP price tools\n    description: >-\n      API key issued from the Pyth Terminal (https://pythdata.app -> View your API key), passed as\n      `Authorization: Bearer {key}`. In the MCP server it is passed as the `access_token` argument.\n      Provider guidance: never embed the key in browser/frontend apps — proxy through your backend.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pyth/refs/heads/main/authentication/pyth-authentication.yml
summary_line: none/http · 3 schemes
tags:
- Company
- Crypto Web3
- Oracle
- Price Feeds
- Market Data
- DeFi
- Blockchain
- Financial Data
---
