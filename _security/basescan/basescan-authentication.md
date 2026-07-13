---
api_key_in:
- query
api_specs:
- filename: openapi.yml
  format: yaml
  label: Basescan API
  slug: basescan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basescan/refs/heads/main/openapi/openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Basescan Authentication
name_suffix: Authentication
oauth_flows: []
overview: Basescan secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Basescan
provider_slug: basescan
scheme_count: 1
schemes:
- in: query
  name: apiKeyAuth
  parameter: apikey
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: basescan-authentication
source_filename: basescan-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: query\n  parameter: apikey\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/basescan/refs/heads/main/authentication/basescan-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- blockchain
- Base
- L2
- explorer
- Ethereum
- EVM
- transactions
- tokens
- smart contracts
---
