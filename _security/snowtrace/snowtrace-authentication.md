---
api_key_in:
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Snowtrace Authentication
name_suffix: Authentication
oauth_flows: []
overview: Routescan (Snowtrace) secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Routescan (Snowtrace)
provider_slug: snowtrace
scheme_count: 1
schemes:
- description: Optional for free-tier usage (2 req/s, 10,000 calls/day). Register at routescan.io for increased limits.
  in: query
  name: apiKey
  parameter: apikey
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: snowtrace-authentication
source_filename: snowtrace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: Optional for free-tier usage (2 req/s, 10,000 calls/day). Register at routescan.io\n    for increased limits.\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snowtrace/refs/heads/main/authentication/snowtrace-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Blockchain
- Explorer
- Avalanche
- EVM
- Multichain
- Web3
- Transactions
- Smart Contracts
- NFTs
- DeFi
---
