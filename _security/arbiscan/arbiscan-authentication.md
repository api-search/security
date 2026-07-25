---
api_key_in:
- query
api_specs:
- filename: arbiscan-accounts-api-openapi.yml
  format: yaml
  label: Arbiscan Accounts API
  slug: arbiscan-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arbiscan/refs/heads/main/openapi/arbiscan-accounts-api-openapi.yml
- filename: arbiscan-blocks-api-openapi.yml
  format: yaml
  label: Arbiscan Blocks API
  slug: arbiscan-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arbiscan/refs/heads/main/openapi/arbiscan-blocks-api-openapi.yml
- filename: arbiscan-contracts-api-openapi.yml
  format: yaml
  label: Arbiscan Contracts API
  slug: arbiscan-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arbiscan/refs/heads/main/openapi/arbiscan-contracts-api-openapi.yml
- filename: arbiscan-gas-tracker-api-openapi.yml
  format: yaml
  label: Arbiscan Gas Tracker API
  slug: arbiscan-gas-tracker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arbiscan/refs/heads/main/openapi/arbiscan-gas-tracker-api-openapi.yml
- filename: arbiscan-logs-api-openapi.yml
  format: yaml
  label: Arbiscan Logs API
  slug: arbiscan-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arbiscan/refs/heads/main/openapi/arbiscan-logs-api-openapi.yml
- filename: arbiscan-stats-api-openapi.yml
  format: yaml
  label: Arbiscan Stats API
  slug: arbiscan-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arbiscan/refs/heads/main/openapi/arbiscan-stats-api-openapi.yml
- filename: arbiscan-tokens-api-openapi.yml
  format: yaml
  label: Arbiscan Tokens API
  slug: arbiscan-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arbiscan/refs/heads/main/openapi/arbiscan-tokens-api-openapi.yml
- filename: arbiscan-transactions-api-openapi.yml
  format: yaml
  label: Arbiscan Transactions API
  slug: arbiscan-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arbiscan/refs/heads/main/openapi/arbiscan-transactions-api-openapi.yml
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
