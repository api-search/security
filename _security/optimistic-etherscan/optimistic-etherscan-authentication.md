---
api_key_in:
- query
api_specs:
- filename: optimistic-etherscan-accounts-api-openapi.yml
  format: yaml
  label: Optimism Etherscan Accounts API
  slug: optimistic-etherscan-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optimistic-etherscan/refs/heads/main/openapi/optimistic-etherscan-accounts-api-openapi.yml
- filename: optimistic-etherscan-blocks-api-openapi.yml
  format: yaml
  label: Optimism Etherscan Blocks API
  slug: optimistic-etherscan-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optimistic-etherscan/refs/heads/main/openapi/optimistic-etherscan-blocks-api-openapi.yml
- filename: optimistic-etherscan-contracts-api-openapi.yml
  format: yaml
  label: Optimism Etherscan Contracts API
  slug: optimistic-etherscan-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optimistic-etherscan/refs/heads/main/openapi/optimistic-etherscan-contracts-api-openapi.yml
- filename: optimistic-etherscan-geth-proxy-api-openapi.yml
  format: yaml
  label: Optimism Etherscan Geth Proxy API
  slug: optimistic-etherscan-geth-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optimistic-etherscan/refs/heads/main/openapi/optimistic-etherscan-geth-proxy-api-openapi.yml
- filename: optimistic-etherscan-stats-api-openapi.yml
  format: yaml
  label: Optimism Etherscan Stats API
  slug: optimistic-etherscan-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optimistic-etherscan/refs/heads/main/openapi/optimistic-etherscan-stats-api-openapi.yml
- filename: optimistic-etherscan-tokens-api-openapi.yml
  format: yaml
  label: Optimism Etherscan Tokens API
  slug: optimistic-etherscan-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optimistic-etherscan/refs/heads/main/openapi/optimistic-etherscan-tokens-api-openapi.yml
- filename: optimistic-etherscan-transactions-api-openapi.yml
  format: yaml
  label: Optimism Etherscan Transactions API
  slug: optimistic-etherscan-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optimistic-etherscan/refs/heads/main/openapi/optimistic-etherscan-transactions-api-openapi.yml
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
