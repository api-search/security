---
api_key_in:
- header
api_specs:
- filename: tatum-openapi.yml
  format: yaml
  label: Tatum Data API
  slug: data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tatum/refs/heads/main/openapi/tatum-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tatum Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tatum secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tatum
provider_slug: tatum
scheme_count: 1
schemes:
- in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/tatum-openapi.yml
  type: apiKey
slug: tatum-authentication
source_filename: tatum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tatum-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/tatum-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tatum/refs/heads/main/authentication/tatum-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Web3
- Blockchain
- RPC
- Multi-chain
- Wallet
- NFT
---
