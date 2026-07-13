---
api_key_in:
- query
api_specs:
- filename: openapi.yml
  format: yaml
  label: BscScan API
  slug: bscscan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bscscan/refs/heads/main/openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Bscscan Authentication
name_suffix: Authentication
oauth_flows: []
overview: BscScan secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BscScan
provider_slug: bscscan
scheme_count: 1
schemes:
- in: query
  name: apiKeyAuth
  parameter: apikey
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: bscscan-authentication
source_filename: bscscan-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: query\n  parameter: apikey\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bscscan/refs/heads/main/authentication/bscscan-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- blockchain
- block-explorer
- BNB Smart Chain
- BSC
- BEP-20
- transactions
- smart-contracts
- DeFi
- EVM
---
