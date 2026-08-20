---
api_key_in:
- query
api_specs:
- filename: bscscan-accounts-api-openapi.yml
  format: yaml
  label: BscScan Accounts API
  slug: bscscan-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bscscan/refs/heads/main/openapi/bscscan-accounts-api-openapi.yml
- filename: bscscan-api-pro-endpoints-api-openapi.yml
  format: yaml
  label: BscScan API PRO Endpoints API
  slug: bscscan-api-pro-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bscscan/refs/heads/main/openapi/bscscan-api-pro-endpoints-api-openapi.yml
- filename: bscscan-blocks-api-openapi.yml
  format: yaml
  label: BscScan Blocks API
  slug: bscscan-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bscscan/refs/heads/main/openapi/bscscan-blocks-api-openapi.yml
- filename: bscscan-contracts-api-openapi.yml
  format: yaml
  label: BscScan Contracts API
  slug: bscscan-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bscscan/refs/heads/main/openapi/bscscan-contracts-api-openapi.yml
- filename: bscscan-gas-tracker-api-openapi.yml
  format: yaml
  label: BscScan Gas Tracker API
  slug: bscscan-gas-tracker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bscscan/refs/heads/main/openapi/bscscan-gas-tracker-api-openapi.yml
- filename: bscscan-geth-parity-proxy-api-openapi.yml
  format: yaml
  label: BscScan Geth/Parity Proxy API
  slug: bscscan-geth-parity-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bscscan/refs/heads/main/openapi/bscscan-geth-parity-proxy-api-openapi.yml
- filename: bscscan-logs-api-openapi.yml
  format: yaml
  label: BscScan Logs API
  slug: bscscan-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bscscan/refs/heads/main/openapi/bscscan-logs-api-openapi.yml
- filename: bscscan-stats-api-openapi.yml
  format: yaml
  label: BscScan Stats API
  slug: bscscan-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bscscan/refs/heads/main/openapi/bscscan-stats-api-openapi.yml
- filename: bscscan-tokens-api-openapi.yml
  format: yaml
  label: BscScan Tokens API
  slug: bscscan-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bscscan/refs/heads/main/openapi/bscscan-tokens-api-openapi.yml
- filename: bscscan-transactions-api-openapi.yml
  format: yaml
  label: BscScan Transactions API
  slug: bscscan-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bscscan/refs/heads/main/openapi/bscscan-transactions-api-openapi.yml
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
- Blockchain
- Block Explorer
- BNB Smart Chain
- BSC
- BEP-20
- Transaction
- Smart Contracts
- DeFi
- EVM
---
