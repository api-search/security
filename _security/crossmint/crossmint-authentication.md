---
api_key_in:
- header
api_specs:
- filename: crossmint-balances-api-openapi.yml
  format: yaml
  label: Crossmint Balances API
  slug: crossmint-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crossmint/refs/heads/main/openapi/crossmint-balances-api-openapi.yml
- filename: crossmint-nfts-api-openapi.yml
  format: yaml
  label: Crossmint NFTs API
  slug: crossmint-nfts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crossmint/refs/heads/main/openapi/crossmint-nfts-api-openapi.yml
- filename: crossmint-signatures-api-openapi.yml
  format: yaml
  label: Crossmint Signatures API
  slug: crossmint-signatures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crossmint/refs/heads/main/openapi/crossmint-signatures-api-openapi.yml
- filename: crossmint-signers-api-openapi.yml
  format: yaml
  label: Crossmint Signers API
  slug: crossmint-signers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crossmint/refs/heads/main/openapi/crossmint-signers-api-openapi.yml
- filename: crossmint-transactions-api-openapi.yml
  format: yaml
  label: Crossmint Transactions API
  slug: crossmint-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crossmint/refs/heads/main/openapi/crossmint-transactions-api-openapi.yml
- filename: crossmint-transfers-api-openapi.yml
  format: yaml
  label: Crossmint Transfers API
  slug: crossmint-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crossmint/refs/heads/main/openapi/crossmint-transfers-api-openapi.yml
- filename: crossmint-wallets-api-openapi.yml
  format: yaml
  label: Crossmint Wallets API
  slug: crossmint-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crossmint/refs/heads/main/openapi/crossmint-wallets-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Crossmint Authentication
name_suffix: Authentication
oauth_flows: []
overview: Crossmint secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Crossmint
provider_slug: crossmint
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/crossmint-openapi.yml
  type: apiKey
slug: crossmint-authentication
source_filename: crossmint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/crossmint-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/crossmint-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crossmint/refs/heads/main/authentication/crossmint-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Web3
- Wallets
- NFT
- Payments
- Checkout
---
