---
api_key_in: []
api_specs:
- filename: circle-nfts-api-openapi.yml
  format: yaml
  label: Circle NFTs API
  slug: circle-nfts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle/refs/heads/main/openapi/circle-nfts-api-openapi.yml
- filename: circle-signing-api-openapi.yml
  format: yaml
  label: Circle Signing API
  slug: circle-signing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle/refs/heads/main/openapi/circle-signing-api-openapi.yml
- filename: circle-tokens-api-openapi.yml
  format: yaml
  label: Circle Tokens API
  slug: circle-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle/refs/heads/main/openapi/circle-tokens-api-openapi.yml
- filename: circle-transactions-api-openapi.yml
  format: yaml
  label: Circle Transactions API
  slug: circle-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle/refs/heads/main/openapi/circle-transactions-api-openapi.yml
- filename: circle-wallet-sets-api-openapi.yml
  format: yaml
  label: Circle Wallet Sets API
  slug: circle-wallet-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle/refs/heads/main/openapi/circle-wallet-sets-api-openapi.yml
- filename: circle-wallets-api-openapi.yml
  format: yaml
  label: Circle Wallets API
  slug: circle-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle/refs/heads/main/openapi/circle-wallets-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Circle Authentication
name_suffix: Authentication
oauth_flows: []
overview: Circle secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Circle
provider_slug: circle
scheme_count: 1
schemes:
- description: Circle API key, formatted as `PREFIX:ID:SECRET`, supplied as Bearer token.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/circle-openapi.yml
  type: http
slug: circle-authentication
source_filename: circle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/circle-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Circle API key, formatted as `PREFIX:ID:SECRET`, supplied as Bearer token.\n  sources:\n  - openapi/circle-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/circle/refs/heads/main/authentication/circle-authentication.yml
summary_line: http · 1 scheme
tags:
- Blockchain
- Compliance
- Cross-Chain
- Currency
- Money
- Payments
- Stablecoin
- Transfers
- USDC
- Wallets
---
