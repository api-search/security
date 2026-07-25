---
api_key_in:
- query
api_specs:
- filename: etherscan-accounts-api-openapi.yml
  format: yaml
  label: Etherscan Accounts API
  slug: etherscan-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/etherscan/refs/heads/main/openapi/etherscan-accounts-api-openapi.yml
- filename: etherscan-blocks-api-openapi.yml
  format: yaml
  label: Etherscan Blocks API
  slug: etherscan-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/etherscan/refs/heads/main/openapi/etherscan-blocks-api-openapi.yml
- filename: etherscan-contracts-api-openapi.yml
  format: yaml
  label: Etherscan Contracts API
  slug: etherscan-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/etherscan/refs/heads/main/openapi/etherscan-contracts-api-openapi.yml
- filename: etherscan-gas-tracker-api-openapi.yml
  format: yaml
  label: Etherscan Gas Tracker API
  slug: etherscan-gas-tracker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/etherscan/refs/heads/main/openapi/etherscan-gas-tracker-api-openapi.yml
- filename: etherscan-stats-api-openapi.yml
  format: yaml
  label: Etherscan Stats API
  slug: etherscan-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/etherscan/refs/heads/main/openapi/etherscan-stats-api-openapi.yml
- filename: etherscan-tokens-api-openapi.yml
  format: yaml
  label: Etherscan Tokens API
  slug: etherscan-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/etherscan/refs/heads/main/openapi/etherscan-tokens-api-openapi.yml
- filename: etherscan-transactions-api-openapi.yml
  format: yaml
  label: Etherscan Transactions API
  slug: etherscan-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/etherscan/refs/heads/main/openapi/etherscan-transactions-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Etherscan Authentication
name_suffix: Authentication
oauth_flows: []
overview: Etherscan secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Etherscan
provider_slug: etherscan
scheme_count: 1
schemes:
- description: Etherscan API key, obtained from https://etherscan.io/myapikey
  in: query
  name: apiKeyAuth
  parameter: apikey
  sources:
  - openapi/etherscan-openapi.yml
  type: apiKey
slug: etherscan-authentication
source_filename: etherscan-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/etherscan-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: Etherscan API key, obtained from https://etherscan.io/myapikey\n  sources:\n  - openapi/etherscan-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/etherscan/refs/heads/main/authentication/etherscan-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Blockchain
- Cryptocurrency
- Ethereum
- EVM
- Web3
---
