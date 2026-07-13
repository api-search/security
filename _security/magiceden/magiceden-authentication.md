---
api_key_in:
- header
api_specs:
- filename: magiceden-openapi.yaml
  format: yaml
  label: Magic Eden Solana Collections API
  slug: magiceden-solana-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magiceden/refs/heads/main/openapi/magiceden-openapi.yaml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Magiceden Authentication
name_suffix: Authentication
oauth_flows: []
overview: Magic Eden secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Magic Eden
provider_slug: magiceden
scheme_count: 3
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-NFT-API-Key
  sources:
  - openapi/magiceden-openapi.yaml
  type: apiKey
- in: header
  name: cookieAuth
  parameter: Cookie
  sources:
  - openapi/magiceden-openapi.yaml
  type: apiKey
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/magiceden-openapi.yaml
  type: http
slug: magiceden-authentication
source_filename: magiceden-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/magiceden-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-NFT-API-Key\n  sources:\n  - openapi/magiceden-openapi.yaml\n- name: cookieAuth\n  type: apiKey\n  in: header\n  parameter: Cookie\n  sources:\n  - openapi/magiceden-openapi.yaml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/magiceden-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/magiceden/refs/heads/main/authentication/magiceden-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- NFT
- NFT Marketplace
- Multi-Chain
- Solana
- Bitcoin
- Ordinals
- Runes
- Ethereum
- Polygon
- Web3
- Blockchain
- DeFi
- Trading
---
