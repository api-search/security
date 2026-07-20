---
api_key_in:
- header
api_specs:
- filename: bitpanda-platform-openapi.yml
  format: yaml
  label: Bitpanda Platform API
  slug: bitpanda-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitpanda/refs/heads/main/openapi/bitpanda-platform-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Bitpanda Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bitpanda secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bitpanda
provider_slug: bitpanda
scheme_count: 1
schemes:
- description: Bitpanda API key. Generate one at https://web.bitpanda.com/my-account/apikey
  in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/bitpanda-platform-openapi.yml
  type: apiKey
slug: bitpanda-authentication
source_filename: bitpanda-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/bitpanda-platform-openapi.yml\ndocs: https://developers.bitpanda.com/platform/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: Bitpanda API key. Generate one at https://web.bitpanda.com/my-account/apikey\n  sources:\n  - openapi/bitpanda-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitpanda/refs/heads/main/authentication/bitpanda-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Cryptocurrency
- Fintech
- Trading
- Investing
- Stocks
- ETFs
- Precious Metals
- Portfolio
- Market Data
- MCP
- Agent Skills
---
