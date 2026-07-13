---
api_key_in:
- header
api_specs:
- filename: openapi.json
  format: json
  label: Bitstamp REST API
  slug: bitstamp-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitstamp/refs/heads/main/openapi/openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Bitstamp Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bitstamp secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Bitstamp
provider_slug: bitstamp
scheme_count: 2
schemes:
- description: Bitstamp API key for authenticated endpoints
  in: header
  name: apiKeyAuth
  parameter: X-Auth
  sources:
  - openapi/openapi.json
  type: apiKey
- description: HMAC-SHA256 request signature
  in: header
  name: apiSignature
  parameter: X-Auth-Signature
  sources:
  - openapi/openapi.json
  type: apiKey
slug: bitstamp-authentication
source_filename: bitstamp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Auth\n  description: Bitstamp API key for authenticated endpoints\n  sources:\n  - openapi/openapi.json\n- name: apiSignature\n  type: apiKey\n  in: header\n  parameter: X-Auth-Signature\n  description: HMAC-SHA256 request signature\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitstamp/refs/heads/main/authentication/bitstamp-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Cryptocurrency
- Exchange
- Trading
- Bitcoin
- Ethereum
- Spot Trading
- WebSocket
- Market Data
- Order Management
- Finance
---
