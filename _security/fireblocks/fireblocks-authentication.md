---
api_key_in:
- header
api_specs:
- filename: fireblocks-vaults-api-openapi.yml
  format: yaml
  label: Fireblocks Vaults API
  slug: fireblocks-vaults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-vaults-api-openapi.yml
- filename: fireblocks-transactions-api-openapi.yml
  format: yaml
  label: Fireblocks Transactions API
  slug: fireblocks-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-transactions-api-openapi.yml
- filename: fireblocks-wallets-api-openapi.yml
  format: yaml
  label: Fireblocks Whitelisted Wallets API
  slug: fireblocks-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-wallets-api-openapi.yml
- filename: fireblocks-assets-api-openapi.yml
  format: yaml
  label: Fireblocks Blockchains and Assets API
  slug: fireblocks-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-assets-api-openapi.yml
- filename: fireblocks-exchange-api-openapi.yml
  format: yaml
  label: Fireblocks Exchange and Fiat Accounts API
  slug: fireblocks-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-exchange-api-openapi.yml
- filename: fireblocks-tokenization-api-openapi.yml
  format: yaml
  label: Fireblocks Tokenization API
  slug: fireblocks-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-tokenization-api-openapi.yml
- filename: fireblocks-contracts-api-openapi.yml
  format: yaml
  label: Fireblocks Smart Contracts API
  slug: fireblocks-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-contracts-api-openapi.yml
- filename: fireblocks-staking-api-openapi.yml
  format: yaml
  label: Fireblocks Staking API
  slug: fireblocks-staking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-staking-api-openapi.yml
- filename: fireblocks-nfts-api-openapi.yml
  format: yaml
  label: Fireblocks NFTs API
  slug: fireblocks-nfts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-nfts-api-openapi.yml
- filename: fireblocks-payments-api-openapi.yml
  format: yaml
  label: Fireblocks Payments API
  slug: fireblocks-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-payments-api-openapi.yml
- filename: fireblocks-network-api-openapi.yml
  format: yaml
  label: Fireblocks Network and Off-Exchange API
  slug: fireblocks-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-network-api-openapi.yml
- filename: fireblocks-compliance-api-openapi.yml
  format: yaml
  label: Fireblocks Compliance and Policy API
  slug: fireblocks-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-compliance-api-openapi.yml
- filename: fireblocks-gas-station-api-openapi.yml
  format: yaml
  label: Fireblocks Gas Station API
  slug: fireblocks-gas-station-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-gas-station-api-openapi.yml
- filename: fireblocks-workspace-api-openapi.yml
  format: yaml
  label: Fireblocks Workspace Management API
  slug: fireblocks-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-workspace-api-openapi.yml
- filename: fireblocks-webhooks-api-openapi.yml
  format: yaml
  label: Fireblocks Webhooks API
  slug: fireblocks-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Fireblocks Authentication
name_suffix: Authentication
oauth_flows: []
overview: fireblocks secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: fireblocks
provider_slug: fireblocks
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearerTokenAuth
  scheme: bearer
  sources:
  - openapi/fireblocks-assets-api-openapi.yml
  - openapi/fireblocks-compliance-api-openapi.yml
  - openapi/fireblocks-contracts-api-openapi.yml
  - openapi/fireblocks-exchange-api-openapi.yml
  - openapi/fireblocks-gas-station-api-openapi.yml
  - openapi/fireblocks-network-api-openapi.yml
  - openapi/fireblocks-nfts-api-openapi.yml
  - openapi/fireblocks-payments-api-openapi.yml
  - openapi/fireblocks-staking-api-openapi.yml
  - openapi/fireblocks-tokenization-api-openapi.yml
  - openapi/fireblocks-transactions-api-openapi.yml
  - openapi/fireblocks-vaults-api-openapi.yml
  - openapi/fireblocks-wallets-api-openapi.yml
  - openapi/fireblocks-webhooks-api-openapi.yml
  - openapi/fireblocks-workspace-api-openapi.yml
  type: http
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/fireblocks-assets-api-openapi.yml
  - openapi/fireblocks-compliance-api-openapi.yml
  - openapi/fireblocks-contracts-api-openapi.yml
  - openapi/fireblocks-exchange-api-openapi.yml
  - openapi/fireblocks-gas-station-api-openapi.yml
  - openapi/fireblocks-network-api-openapi.yml
  - openapi/fireblocks-nfts-api-openapi.yml
  - openapi/fireblocks-payments-api-openapi.yml
  - openapi/fireblocks-staking-api-openapi.yml
  - openapi/fireblocks-tokenization-api-openapi.yml
  - openapi/fireblocks-transactions-api-openapi.yml
  - openapi/fireblocks-vaults-api-openapi.yml
  - openapi/fireblocks-wallets-api-openapi.yml
  - openapi/fireblocks-webhooks-api-openapi.yml
  - openapi/fireblocks-workspace-api-openapi.yml
  type: apiKey
slug: fireblocks-authentication
source_filename: fireblocks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fireblocks-assets-api-openapi.yml, openapi/fireblocks-compliance-api-openapi.yml,\n  openapi/fireblocks-contracts-api-openapi.yml, openapi/fireblocks-exchange-api-openapi.yml,\n  openapi/fireblocks-gas-station-api-openapi.yml, openapi/fireblocks-network-api-openapi.yml,\n  openapi/fireblocks-nfts-api-openapi.yml, openapi/fireblocks-payments-api-openapi.yml, openapi/fireblocks-staking-api-openapi.yml,\n  openapi/fireblocks-tokenization-api-openapi.yml, openapi/fireblocks-transactions-api-openapi.yml,\n  openapi/fireblocks-vaults-api-openapi.yml ...\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerTokenAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/fireblocks-assets-api-openapi.yml\n  - openapi/fireblocks-compliance-api-openapi.yml\n  - openapi/fireblocks-contracts-api-openapi.yml\n  - openapi/fireblocks-exchange-api-openapi.yml\n  - openapi/fireblocks-gas-station-api-openapi.yml\n\
  \  - openapi/fireblocks-network-api-openapi.yml\n  - openapi/fireblocks-nfts-api-openapi.yml\n  - openapi/fireblocks-payments-api-openapi.yml\n  - openapi/fireblocks-staking-api-openapi.yml\n  - openapi/fireblocks-tokenization-api-openapi.yml\n  - openapi/fireblocks-transactions-api-openapi.yml\n  - openapi/fireblocks-vaults-api-openapi.yml\n  - openapi/fireblocks-wallets-api-openapi.yml\n  - openapi/fireblocks-webhooks-api-openapi.yml\n  - openapi/fireblocks-workspace-api-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/fireblocks-assets-api-openapi.yml\n  - openapi/fireblocks-compliance-api-openapi.yml\n  - openapi/fireblocks-contracts-api-openapi.yml\n  - openapi/fireblocks-exchange-api-openapi.yml\n  - openapi/fireblocks-gas-station-api-openapi.yml\n  - openapi/fireblocks-network-api-openapi.yml\n  - openapi/fireblocks-nfts-api-openapi.yml\n  - openapi/fireblocks-payments-api-openapi.yml\n  - openapi/fireblocks-staking-api-openapi.yml\n\
  \  - openapi/fireblocks-tokenization-api-openapi.yml\n  - openapi/fireblocks-transactions-api-openapi.yml\n  - openapi/fireblocks-vaults-api-openapi.yml\n  - openapi/fireblocks-wallets-api-openapi.yml\n  - openapi/fireblocks-webhooks-api-openapi.yml\n  - openapi/fireblocks-workspace-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/authentication/fireblocks-authentication.yml
summary_line: apiKey/http · 2 schemes
tags: []
---
