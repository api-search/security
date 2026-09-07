---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: parlay-api-openapi.json
  format: json
  label: ParlayAPI
  slug: parlayapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parlay-api/refs/heads/main/openapi/parlay-api-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Parlay Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: ParlayAPI secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ParlayAPI
provider_slug: parlay-api
scheme_count: 3
schemes:
- description: API key passed in the X-API-Key header. Recommended.
  in: header
  name: apiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/parlay-api-openapi.json
  type: apiKey
- description: API key passed as the ?apiKey= query parameter. Useful for browser fetch() and webhooks where header control is limited. Equivalent to X-API-Key.
  in: query
  name: apiKeyQuery
  parameter: apiKey
  sources:
  - openapi/parlay-api-openapi.json
  type: apiKey
- bearerFormat: APIKey
  description: 'API key passed via Authorization: Bearer <key>. Equivalent to X-API-Key for compatibility with auth libraries that expect bearer tokens.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/parlay-api-openapi.json
  type: http
slug: parlay-api-authentication
source_filename: parlay-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: derived\nsource: openapi/parlay-api-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key passed in the X-API-Key header. Recommended.\n  sources:\n  - openapi/parlay-api-openapi.json\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: apiKey\n  description: API key passed as the ?apiKey= query parameter. Useful for browser fetch() and\n    webhooks where header control is limited. Equivalent to X-API-Key.\n  sources:\n  - openapi/parlay-api-openapi.json\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: APIKey\n  description: 'API key passed via Authorization: Bearer <key>. Equivalent to X-API-Key for\n    compatibility with auth libraries that expect bearer tokens.'\n  sources:\n  - openapi/parlay-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parlay-api/refs/heads/main/authentication/parlay-api-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Sports
- Odds
- Betting Data
- Sports Data
- Prediction Markets
- Player Props
- Arbitrage
- Streaming
---
