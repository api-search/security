---
api_key_in:
- header
auth_types:
- apiKey
- http
- signed-request
- jwt
description: ''
kind: authentication
layout: security
method: searched
name: Mammoth Media Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mammoth Media secures its APIs with apiKey, http, signed-request, and jwt across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Mammoth Media
provider_slug: mammoth-media
scheme_count: 5
schemes:
- applies_to: REST API
  in: header
  key_format:
    production: tb_live_<...>
    test: tb_test_<...>
  name: apiKey
  parameter_name: X-API-Key
  permissions:
  - ADMIN required for /v1/api-keys management
  type: apiKey
- applies_to: REST API
  name: bearer
  note: Authorization Bearer value is interpreted as an API key (no standalone JWT verification on REST).
  scheme: bearer
  type: http
- applies_to: REST API + GraphQL (CLI fast-path)
  canonical_string: ${METHOD}\n${path}\n${timestamp}\n${nonce}\n${sha256(body)}
  headers:
  - x-tb-pubkey
  - x-tb-timestamp
  - x-tb-nonce
  - x-tb-sig
  implemented_by: '@tokenbot-org/cli-core'
  name: signed-request
  replay_protection:
    clock_skew: +/-60 seconds
    nonce_window: 10 minutes
  scheme: secp256k1
  type: signed-request
- applies_to: GraphQL API
  bearer_format: JWT
  name: jwt
  note: JWT obtained from the login mutation.
  scheme: bearer
  type: http
- applies_to: MCP server -> GraphQL backend
  companion_header: X-User-Id
  in: header
  name: mcp-service-token
  parameter_name: X-Service-Token
  type: apiKey
slug: mammoth-media-authentication
source_filename: mammoth-media-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.tokenbot.com/home/api-docs/authentication\ndocs: https://docs.tokenbot.com/home/api-docs/authentication\nsummary:\n  types: [apiKey, http, signed-request, jwt]\n  api_key_in: [header]\n  api_key_headers: [X-API-Key, Authorization]\n  notes: >-\n    REST API accepts an API key via X-API-Key or Authorization: Bearer (the\n    bearer value is treated as an API key, not a verified JWT). The tokenbot CLI\n    uses a secp256k1 signed-request fast-path. The GraphQL API accepts a JWT\n    bearer token (from login) or the CLI signed request.\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter_name: X-API-Key\n  applies_to: REST API\n  key_format:\n    production: tb_live_<...>\n    test: tb_test_<...>\n  permissions: [ADMIN required for /v1/api-keys management]\n- name: bearer\n  type: http\n  scheme: bearer\n  applies_to: REST API\n  note: Authorization Bearer value is interpreted as an API key (no standalone\
  \ JWT verification on REST).\n- name: signed-request\n  type: signed-request\n  scheme: secp256k1\n  applies_to: REST API + GraphQL (CLI fast-path)\n  headers:\n  - x-tb-pubkey\n  - x-tb-timestamp\n  - x-tb-nonce\n  - x-tb-sig\n  canonical_string: \"${METHOD}\\\\n${path}\\\\n${timestamp}\\\\n${nonce}\\\\n${sha256(body)}\"\n  replay_protection:\n    clock_skew: \"+/-60 seconds\"\n    nonce_window: 10 minutes\n  implemented_by: \"@tokenbot-org/cli-core\"\n- name: jwt\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  applies_to: GraphQL API\n  note: JWT obtained from the login mutation.\n- name: mcp-service-token\n  type: apiKey\n  in: header\n  parameter_name: X-Service-Token\n  applies_to: MCP server -> GraphQL backend\n  companion_header: X-User-Id\npublic_endpoints:\n- GET /v1/health\n- GET /v1/health/detailed\n- GET /v1/version\n- GET /v1/auth/cli-challenge\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mammoth-media/refs/heads/main/authentication/mammoth-media-authentication.yml
summary_line: apiKey/http/signed-request/jwt · 5 schemes
tags:
- Company
- Consumer
- Cryptocurrency
- Trading
- Copy Trading
- Fintech
- Webhooks
- MCP
- Developer Tools
- CLI
---
