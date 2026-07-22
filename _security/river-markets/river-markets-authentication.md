---
api_key_in:
- header
api_specs:
- filename: river-markets-openapi-original.json
  format: json
  label: River Markets API
  slug: river-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/river-markets/refs/heads/main/openapi/river-markets-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: River Markets Authentication
name_suffix: Authentication
oauth_flows: []
overview: River Markets secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: River Markets
provider_slug: river-markets
scheme_count: 4
schemes:
- description: UUID of your API key (from Settings → API Keys).
  in: header
  name: SignedRequestKeyId
  parameter: X-River-Key-Id
  sources:
  - openapi/river-markets-openapi-original.json
  type: apiKey
- description: Current unix seconds. Must be within 30s of server time.
  in: header
  name: SignedRequestTimestamp
  parameter: X-River-Timestamp
  sources:
  - openapi/river-markets-openapi-original.json
  type: apiKey
- description: 'Base64 Ed25519 signature over the canonical request: METHOD\nPATH\nSORTED_QUERY\nTIMESTAMP\nSHA256(body) hex. See /api-reference/authentication for the full recipe.'
  in: header
  name: SignedRequestSignature
  parameter: X-River-Signature
  sources:
  - openapi/river-markets-openapi-original.json
  type: apiKey
- description: JWT bearer token for web client authentication.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/river-markets-openapi-original.json
  type: http
slug: river-markets-authentication
source_filename: river-markets-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/river-markets-openapi-original.json\ndocs: https://docs.rivermarkets.com/api-reference/authentication\nnotes: >-\n  Primary programmatic auth is Ed25519 request signing via three apiKey headers\n  (X-River-Key-Id, X-River-Timestamp, X-River-Signature). The canonical string is\n  LF-joined: METHOD\\nPATH\\nSORTED_QUERY\\nTIMESTAMP\\nSHA256(body) hex. Timestamp must\n  be within 30s of server time; signatures are deduped in Redis with a 60s TTL for\n  replay protection. Keys are asymmetric — the server stores only the public key and\n  the private key is shown once at creation and never traverses the wire after that.\n  BearerAuth (JWT) is used by the web client. The official Python SDK signs transparently.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: SignedRequestKeyId\n  type: apiKey\n  in: header\n  parameter: X-River-Key-Id\n  description: UUID of your API key (from Settings\
  \ → API Keys).\n  sources:\n  - openapi/river-markets-openapi-original.json\n- name: SignedRequestTimestamp\n  type: apiKey\n  in: header\n  parameter: X-River-Timestamp\n  description: Current unix seconds. Must be within 30s of server time.\n  sources:\n  - openapi/river-markets-openapi-original.json\n- name: SignedRequestSignature\n  type: apiKey\n  in: header\n  parameter: X-River-Signature\n  description: 'Base64 Ed25519 signature over the canonical request: METHOD\\nPATH\\nSORTED_QUERY\\nTIMESTAMP\\nSHA256(body)\n    hex. See /api-reference/authentication for the full recipe.'\n  sources:\n  - openapi/river-markets-openapi-original.json\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: JWT bearer token for web client authentication.\n  sources:\n  - openapi/river-markets-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/river-markets/refs/heads/main/authentication/river-markets-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Company
- Prediction Markets
- Trading
- Prime Brokerage
- Financial Services
- Order Management
- Market Data
- WebSocket
- Fintech
---
