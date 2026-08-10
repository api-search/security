---
api_key_in:
- header
api_specs:
- filename: wealthville-defi-liquidity-pool-scores-api-solana-evm-scores-api-openapi.yml
  format: yaml
  label: WealthVille — DeFi Liquidity Pool Scores API (Solana & EVM) Scores API
  slug: wealthville-defi-liquidity-pool-scores-api-solana-evm-scores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wealthville-defi-liquidity-pool-scores-api-solana-evm/refs/heads/main/openapi/wealthville-defi-liquidity-pool-scores-api-solana-evm-scores-api-openapi.yml
- filename: wealthville-defi-liquidity-pool-scores-api-solana-evm-signals-api-openapi.yml
  format: yaml
  label: WealthVille — DeFi Liquidity Pool Scores API (Solana & EVM) Signals API
  slug: wealthville-defi-liquidity-pool-scores-api-solana-evm-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wealthville-defi-liquidity-pool-scores-api-solana-evm/refs/heads/main/openapi/wealthville-defi-liquidity-pool-scores-api-solana-evm-signals-api-openapi.yml
- filename: wealthville-defi-liquidity-pool-scores-api-solana-evm-track-record-api-openapi.yml
  format: yaml
  label: WealthVille — DeFi Liquidity Pool Scores API (Solana & EVM) Track Record API
  slug: wealthville-defi-liquidity-pool-scores-api-solana-evm-track-record-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wealthville-defi-liquidity-pool-scores-api-solana-evm/refs/heads/main/openapi/wealthville-defi-liquidity-pool-scores-api-solana-evm-track-record-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Wealthville Defi Liquidity Pool Scores Api Solana Evm Authentication
name_suffix: Authentication
oauth_flows: []
overview: WealthVille — DeFi Liquidity Pool Scores API (Solana & EVM) secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: WealthVille — DeFi Liquidity Pool Scores API (Solana & EVM)
provider_slug: wealthville-defi-liquidity-pool-scores-api-solana-evm
scheme_count: 1
schemes:
- description: Optional partner key — raises the rate limit and identifies the caller.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/wealthville-defi-liquidity-pool-scores-api-solana-evm-public-data-openapi.json
  type: apiKey
slug: wealthville-defi-liquidity-pool-scores-api-solana-evm-authentication
source_filename: wealthville-defi-liquidity-pool-scores-api-solana-evm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: derived\nsource: openapi/wealthville-defi-liquidity-pool-scores-api-solana-evm-public-data-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Optional partner key — raises the rate limit and identifies the caller.\n  sources:\n  - openapi/wealthville-defi-liquidity-pool-scores-api-solana-evm-public-data-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wealthville-defi-liquidity-pool-scores-api-solana-evm/refs/heads/main/authentication/wealthville-defi-liquidity-pool-scores-api-solana-evm-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- DeFi
- Liquidity Pools
- Blockchain Analytics
- Solana
- EVM
- Ethereum
- Yield Farming
- Risk Scoring
- MCP
- AI Agents
- Financial Data
---
