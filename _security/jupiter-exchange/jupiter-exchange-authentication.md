---
api_key_in:
- header
api_specs:
- filename: jupiter-exchange-openapi.yml
  format: yaml
  label: Jupiter Swap API
  slug: swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupiter-exchange/refs/heads/main/openapi/jupiter-exchange-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Jupiter Exchange Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jupiter secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Jupiter
provider_slug: jupiter-exchange
scheme_count: 1
schemes:
- description: Jupiter API key issued via the Jupiter Developer Platform.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/jupiter-exchange-openapi.yml
  type: apiKey
slug: jupiter-exchange-authentication
source_filename: jupiter-exchange-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/jupiter-exchange-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Jupiter API key issued via the Jupiter Developer Platform.\n  sources:\n  - openapi/jupiter-exchange-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jupiter-exchange/refs/heads/main/authentication/jupiter-exchange-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Web3
- Solana
- DEX
- Aggregator
- Swap
- Limit Orders
- DCA
- Perpetuals
---
