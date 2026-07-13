---
api_key_in:
- query
api_specs:
- filename: arbiscan-openapi.yml
  format: yaml
  label: Arbiscan API
  slug: arbiscan
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arbiscan/refs/heads/main/openapi/arbiscan-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Arbiscan Authentication
name_suffix: Authentication
oauth_flows: []
overview: Arbiscan secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Arbiscan
provider_slug: arbiscan
scheme_count: 1
schemes:
- description: Etherscan V2 API key from https://arbiscan.io/myapikey
  in: query
  name: apiKeyAuth
  parameter: apikey
  sources:
  - openapi/arbiscan-openapi.yml
  type: apiKey
slug: arbiscan-authentication
source_filename: arbiscan-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/arbiscan-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: Etherscan V2 API key from https://arbiscan.io/myapikey\n  sources:\n  - openapi/arbiscan-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arbiscan/refs/heads/main/authentication/arbiscan-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Blockchain
- Cryptocurrency
- Arbitrum
- Layer 2
- EVM
- Web3
- L2
---
