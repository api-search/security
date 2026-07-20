---
api_key_in:
- query
api_specs:
- filename: dodo-trade-openapi.yml
  format: yaml
  label: DODO Trade / Route API
  slug: dodo-trade-route-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dodo/refs/heads/main/openapi/dodo-trade-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Dodo Authentication
name_suffix: Authentication
oauth_flows: []
overview: DODO secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DODO
provider_slug: dodo
scheme_count: 1
schemes:
- description: API key issued by the DODO Developer Portal (https://docs.dodoex.io/en/developer), passed as the `apikey` query parameter on production Route API requests.
  in: query
  name: apiKeyQuery
  parameter: apikey
  sources:
  - openapi/dodo-trade-openapi.yml
  type: apiKey
slug: dodo-authentication
source_filename: dodo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/dodo-trade-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: API key issued by the DODO Developer Portal (https://docs.dodoex.io/en/developer),\n    passed as the `apikey` query parameter on production Route API requests.\n  sources:\n  - openapi/dodo-trade-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dodo/refs/heads/main/authentication/dodo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Crypto
- DeFi
- DEX
- Decentralized Exchange
- Blockchain
- Trading
- Liquidity
- Web3
- Swap
---
