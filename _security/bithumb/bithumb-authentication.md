---
api_key_in:
- query
api_specs:
- filename: llms.txt
  format: yaml
  label: Bithumb REST API
  slug: bithumb-rest-api
  spec_type: OpenAPI
  url: https://apidocs.bithumb.com/llms.txt
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Bithumb Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bithumb secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bithumb
provider_slug: bithumb
scheme_count: 1
schemes:
- description: API key issued from bithumb.pro. All authenticated requests must also include `timestamp` (Unix ms) and `signature` (HmacSHA256 of sorted request parameters joined with "&").
  in: query
  name: ApiKeyAuth
  parameter: apiKey
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: bithumb-authentication
source_filename: bithumb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: apiKey\n  description: API key issued from bithumb.pro. All authenticated requests must also include\n    `timestamp` (Unix ms) and `signature` (HmacSHA256 of sorted request parameters joined with\n    \"&\").\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bithumb/refs/heads/main/authentication/bithumb-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cryptocurrency
- Exchange
- Trading
- South Korea
- KRW
- Bitcoin
- Market Data
- WebSocket
---
