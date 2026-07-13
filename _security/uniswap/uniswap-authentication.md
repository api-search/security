---
api_key_in:
- header
api_specs:
- filename: uniswap-trading-openapi.yaml
  format: yaml
  label: Uniswap Trading API
  slug: uniswap-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uniswap/refs/heads/main/openapi/uniswap-trading-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Uniswap Authentication
name_suffix: Authentication
oauth_flows: []
overview: Uniswap secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Uniswap
provider_slug: uniswap
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/uniswap-trading-openapi.json
  - openapi/uniswap-trading-openapi.yaml
  type: apiKey
slug: uniswap-authentication
source_filename: uniswap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/uniswap-trading-openapi.json, openapi/uniswap-trading-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/uniswap-trading-openapi.json\n  - openapi/uniswap-trading-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uniswap/refs/heads/main/authentication/uniswap-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Blockchain
- Cryptocurrency
- DeFi
- Decentralized Exchange
- Liquidity
- Swaps
---
