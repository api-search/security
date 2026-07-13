---
api_key_in:
- header
api_specs:
- filename: docs
  format: yaml
  label: Zora Coins SDK REST API
  slug: coins-rest-api
  spec_type: OpenAPI
  url: https://api-sdk.zora.engineering/docs
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Zora Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zora secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zora
provider_slug: zora
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: api-key
  sources:
  - openapi/zora-coins-rest-api-openapi.json
  type: apiKey
slug: zora-authentication
source_filename: zora-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zora-coins-rest-api-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: api-key\n  sources:\n  - openapi/zora-coins-rest-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zora/refs/heads/main/authentication/zora-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- NFT
- Web3
- Blockchain
- Ethereum
- L2
- Creator Economy
- Marketplace
- Zora Network
- Base
- Optimism
---
