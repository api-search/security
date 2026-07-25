---
api_key_in: []
api_specs:
- filename: zerion-chains-api-openapi.yml
  format: yaml
  label: Zerion chains API
  slug: zerion-chains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerion/refs/heads/main/openapi/zerion-chains-api-openapi.yml
- filename: zerion-dapps-api-openapi.yml
  format: yaml
  label: Zerion dapps API
  slug: zerion-dapps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerion/refs/heads/main/openapi/zerion-dapps-api-openapi.yml
- filename: zerion-fungibles-api-openapi.yml
  format: yaml
  label: Zerion fungibles API
  slug: zerion-fungibles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerion/refs/heads/main/openapi/zerion-fungibles-api-openapi.yml
- filename: zerion-gas-api-openapi.yml
  format: yaml
  label: Zerion gas API
  slug: zerion-gas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerion/refs/heads/main/openapi/zerion-gas-api-openapi.yml
- filename: zerion-nfts-api-openapi.yml
  format: yaml
  label: Zerion nfts API
  slug: zerion-nfts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerion/refs/heads/main/openapi/zerion-nfts-api-openapi.yml
- filename: zerion-subscriptions-to-transactions-api-openapi.yml
  format: yaml
  label: Zerion subscriptions to transactions API
  slug: zerion-subscriptions-to-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerion/refs/heads/main/openapi/zerion-subscriptions-to-transactions-api-openapi.yml
- filename: zerion-swap-api-openapi.yml
  format: yaml
  label: Zerion swap API
  slug: zerion-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerion/refs/heads/main/openapi/zerion-swap-api-openapi.yml
- filename: zerion-wallet-sets-api-openapi.yml
  format: yaml
  label: Zerion wallet sets API
  slug: zerion-wallet-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerion/refs/heads/main/openapi/zerion-wallet-sets-api-openapi.yml
- filename: zerion-wallets-api-openapi.yml
  format: yaml
  label: Zerion wallets API
  slug: zerion-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerion/refs/heads/main/openapi/zerion-wallets-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Zerion Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zerion secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zerion
provider_slug: zerion
scheme_count: 1
schemes:
- description: To test endpoints here, paste your API key from the [dashboard](https://dashboard.zerion.io/) into the username field and leave the password empty.
  name: APIKeyBasicAuth
  scheme: basic
  sources:
  - openapi/zerion-openapi-original.yml
  type: http
slug: zerion-authentication
source_filename: zerion-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/zerion-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: APIKeyBasicAuth\n  type: http\n  scheme: basic\n  description: To test endpoints here, paste your API key from the [dashboard](https://dashboard.zerion.io/)\n    into the username field and leave the password empty.\n  sources:\n  - openapi/zerion-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zerion/refs/heads/main/authentication/zerion-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Web3
- Blockchain
- Cryptocurrency
- DeFi
- Wallet
- NFT
- Ethereum
- Solana
- Portfolio
- Onchain Data
- Transactions
---
