---
api_key_in:
- query
api_specs:
- filename: optimistic-etherscan-openapi.yml
  format: yaml
  label: Optimism Etherscan API
  slug: optimistic-etherscan
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optimistic-etherscan/refs/heads/main/openapi/optimistic-etherscan-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Optimistic Etherscan Authentication
name_suffix: Authentication
oauth_flows: []
overview: Optimism Etherscan secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Optimism Etherscan
provider_slug: optimistic-etherscan
scheme_count: 1
schemes:
- description: Etherscan API key obtained from https://optimistic.etherscan.io/myapikey. The free tier supports select chains with 3 req/s and 100k req/day. Paid plans start at $49/month for full multichain access.
  in: query
  name: apiKeyAuth
  parameter: apikey
  sources:
  - openapi/optimistic-etherscan-openapi.yml
  type: apiKey
slug: optimistic-etherscan-authentication
source_filename: optimistic-etherscan-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/optimistic-etherscan-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: Etherscan API key obtained from https://optimistic.etherscan.io/myapikey. The\n    free tier supports select chains with 3 req/s and 100k req/day. Paid plans start at $49/month\n    for full multichain access.\n  sources:\n  - openapi/optimistic-etherscan-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optimistic-etherscan/refs/heads/main/authentication/optimistic-etherscan-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Blockchain
- Optimism
- Layer 2
- Ethereum
- EVM
- Web3
- Cryptocurrency
---
