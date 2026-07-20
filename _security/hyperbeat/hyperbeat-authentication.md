---
api_key_in: []
api_specs:
- filename: hyperbeat-staking-openapi.yml
  format: yaml
  label: Hyperbeat Staking API
  slug: hyperbeat-staking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperbeat/refs/heads/main/openapi/hyperbeat-staking-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hyperbeat Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hyperbeat secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hyperbeat
provider_slug: hyperbeat
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearer
  scheme: bearer
  sources:
  - openapi/hyperbeat-staking-openapi.yml
  type: http
slug: hyperbeat-authentication
source_filename: hyperbeat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/hyperbeat-staking-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/hyperbeat-staking-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperbeat/refs/heads/main/authentication/hyperbeat-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- DeFi
- Staking
- Liquid Staking
- Hyperliquid
- HyperEVM
- Blockchain
- Web3
- Cryptocurrency
- Yield
---
