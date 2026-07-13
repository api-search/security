---
api_key_in:
- header
api_specs:
- filename: nansen-openapi.yml
  format: yaml
  label: Nansen REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nansen/refs/heads/main/openapi/nansen-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Nansen Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nansen secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nansen
provider_slug: nansen
scheme_count: 1
schemes:
- description: Nansen API key issued to subscribed customers.
  in: header
  name: apiKeyAuth
  parameter: apiKey
  sources:
  - openapi/nansen-openapi.yml
  type: apiKey
slug: nansen-authentication
source_filename: nansen-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nansen-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: apiKey\n  description: Nansen API key issued to subscribed customers.\n  sources:\n  - openapi/nansen-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nansen/refs/heads/main/authentication/nansen-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Web3
- Crypto
- On-Chain
- Wallet Labels
- Smart Money
- Analytics
- Multi-chain
---
