---
api_key_in:
- header
api_specs:
- filename: crossmint-openapi.yml
  format: yaml
  label: Crossmint Wallets API
  slug: wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crossmint/refs/heads/main/openapi/crossmint-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Crossmint Authentication
name_suffix: Authentication
oauth_flows: []
overview: Crossmint secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Crossmint
provider_slug: crossmint
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/crossmint-openapi.yml
  type: apiKey
slug: crossmint-authentication
source_filename: crossmint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/crossmint-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/crossmint-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crossmint/refs/heads/main/authentication/crossmint-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Web3
- Wallets
- NFT
- Payments
- Checkout
---
