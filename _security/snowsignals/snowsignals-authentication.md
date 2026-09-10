---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: snowsignals-daas-openapi.json
  format: json
  label: SnowSignals API
  slug: snowsignals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snowsignals/refs/heads/main/openapi/snowsignals-daas-openapi.json
- filename: snowsignals-x402-openapi.json
  format: json
  label: SnowSignals x402 Gateway
  slug: snowsignals-x402-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snowsignals/refs/heads/main/openapi/snowsignals-x402-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Snowsignals Authentication
name_suffix: Authentication
oauth_flows: []
overview: SnowSignals secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SnowSignals
provider_slug: snowsignals
scheme_count: 2
schemes:
- description: 'url method (default): pass your key as `?apiKey=<key>`. The key is the whole credential.'
  in: query
  name: UrlKey
  parameter: apiKey
  sources:
  - openapi/snowsignals-daas-openapi.json
  type: apiKey
- description: 'nonce method: `ApiKey base64(key:nonce:proof)` where `proof = SHA256("secret:nonce")` hex truncated to 19 chars (see the API description for the signing scheme).'
  in: header
  name: ApiKey
  parameter: Authorization
  sources:
  - openapi/snowsignals-daas-openapi.json
  type: apiKey
slug: snowsignals-authentication
source_filename: snowsignals-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: derived\nsource: openapi/snowsignals-daas-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: UrlKey\n  type: apiKey\n  in: query\n  parameter: apiKey\n  description: 'url method (default): pass your key as `?apiKey=<key>`. The key is the whole\n    credential.'\n  sources:\n  - openapi/snowsignals-daas-openapi.json\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'nonce method: `ApiKey base64(key:nonce:proof)` where `proof = SHA256(\"secret:nonce\")`\n    hex truncated to 19 chars (see the API description for the signing scheme).'\n  sources:\n  - openapi/snowsignals-daas-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snowsignals/refs/heads/main/authentication/snowsignals-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- crypto
- market-data
- bitcoin
- analytics
- market-phase
- regime
- trendvane
- daas
- mcp
- agent-native
- financial-data
- x402
---
