---
api_key_in:
- query
api_specs:
- filename: snowtrace-accounts-api-openapi.yml
  format: yaml
  label: Routescan (Snowtrace) Accounts API
  slug: snowtrace-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snowtrace/refs/heads/main/openapi/snowtrace-accounts-api-openapi.yml
- filename: snowtrace-blocks-api-openapi.yml
  format: yaml
  label: Routescan (Snowtrace) Blocks API
  slug: snowtrace-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snowtrace/refs/heads/main/openapi/snowtrace-blocks-api-openapi.yml
- filename: snowtrace-contracts-api-openapi.yml
  format: yaml
  label: Routescan (Snowtrace) Contracts API
  slug: snowtrace-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snowtrace/refs/heads/main/openapi/snowtrace-contracts-api-openapi.yml
- filename: snowtrace-logs-api-openapi.yml
  format: yaml
  label: Routescan (Snowtrace) Logs API
  slug: snowtrace-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snowtrace/refs/heads/main/openapi/snowtrace-logs-api-openapi.yml
- filename: snowtrace-proxy-api-openapi.yml
  format: yaml
  label: Routescan (Snowtrace) Proxy API
  slug: snowtrace-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snowtrace/refs/heads/main/openapi/snowtrace-proxy-api-openapi.yml
- filename: snowtrace-stats-api-openapi.yml
  format: yaml
  label: Routescan (Snowtrace) Stats API
  slug: snowtrace-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snowtrace/refs/heads/main/openapi/snowtrace-stats-api-openapi.yml
- filename: snowtrace-tokens-api-openapi.yml
  format: yaml
  label: Routescan (Snowtrace) Tokens API
  slug: snowtrace-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snowtrace/refs/heads/main/openapi/snowtrace-tokens-api-openapi.yml
- filename: snowtrace-transactions-api-openapi.yml
  format: yaml
  label: Routescan (Snowtrace) Transactions API
  slug: snowtrace-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snowtrace/refs/heads/main/openapi/snowtrace-transactions-api-openapi.yml
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
- Multi-Chain
- Web3
- Transaction
- Smart Contracts
- NFT
- DeFi
---
