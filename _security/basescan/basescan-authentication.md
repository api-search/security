---
api_key_in:
- query
api_specs:
- filename: basescan-accounts-api-openapi.yml
  format: yaml
  label: Basescan Accounts API
  slug: basescan-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basescan/refs/heads/main/openapi/basescan-accounts-api-openapi.yml
- filename: basescan-api-pro-endpoints-api-openapi.yml
  format: yaml
  label: Basescan API PRO Endpoints API
  slug: basescan-api-pro-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basescan/refs/heads/main/openapi/basescan-api-pro-endpoints-api-openapi.yml
- filename: basescan-blocks-api-openapi.yml
  format: yaml
  label: Basescan Blocks API
  slug: basescan-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basescan/refs/heads/main/openapi/basescan-blocks-api-openapi.yml
- filename: basescan-contracts-api-openapi.yml
  format: yaml
  label: Basescan Contracts API
  slug: basescan-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basescan/refs/heads/main/openapi/basescan-contracts-api-openapi.yml
- filename: basescan-gas-tracker-api-openapi.yml
  format: yaml
  label: Basescan Gas Tracker API
  slug: basescan-gas-tracker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basescan/refs/heads/main/openapi/basescan-gas-tracker-api-openapi.yml
- filename: basescan-geth-parity-proxy-api-openapi.yml
  format: yaml
  label: Basescan Geth/Parity Proxy API
  slug: basescan-geth-parity-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basescan/refs/heads/main/openapi/basescan-geth-parity-proxy-api-openapi.yml
- filename: basescan-logs-api-openapi.yml
  format: yaml
  label: Basescan Logs API
  slug: basescan-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basescan/refs/heads/main/openapi/basescan-logs-api-openapi.yml
- filename: basescan-stats-api-openapi.yml
  format: yaml
  label: Basescan Stats API
  slug: basescan-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basescan/refs/heads/main/openapi/basescan-stats-api-openapi.yml
- filename: basescan-tokens-api-openapi.yml
  format: yaml
  label: Basescan Tokens API
  slug: basescan-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basescan/refs/heads/main/openapi/basescan-tokens-api-openapi.yml
- filename: basescan-transactions-api-openapi.yml
  format: yaml
  label: Basescan Transactions API
  slug: basescan-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basescan/refs/heads/main/openapi/basescan-transactions-api-openapi.yml
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
- Blockchain
- Base
- L2
- explorer
- Ethereum
- EVM
- Transaction
- Tokens
- smart contracts
---
