---
api_key_in:
- cookie
- header
api_specs:
- filename: gnosis-safe-4337-api-openapi.yml
  format: yaml
  label: Safe (Gnosis Safe) 4337 API
  slug: gnosis-safe-4337-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gnosis-safe/refs/heads/main/openapi/gnosis-safe-4337-api-openapi.yml
- filename: gnosis-safe-about-api-openapi.yml
  format: yaml
  label: Safe (Gnosis Safe) about API
  slug: gnosis-safe-about-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gnosis-safe/refs/heads/main/openapi/gnosis-safe-about-api-openapi.yml
- filename: gnosis-safe-analytics-api-openapi.yml
  format: yaml
  label: Safe (Gnosis Safe) analytics API
  slug: gnosis-safe-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gnosis-safe/refs/heads/main/openapi/gnosis-safe-analytics-api-openapi.yml
- filename: gnosis-safe-contracts-api-openapi.yml
  format: yaml
  label: Safe (Gnosis Safe) contracts API
  slug: gnosis-safe-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gnosis-safe/refs/heads/main/openapi/gnosis-safe-contracts-api-openapi.yml
- filename: gnosis-safe-data-decoder-api-openapi.yml
  format: yaml
  label: Safe (Gnosis Safe) data-decoder API
  slug: gnosis-safe-data-decoder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gnosis-safe/refs/heads/main/openapi/gnosis-safe-data-decoder-api-openapi.yml
- filename: gnosis-safe-delegates-api-openapi.yml
  format: yaml
  label: Safe (Gnosis Safe) delegates API
  slug: gnosis-safe-delegates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gnosis-safe/refs/heads/main/openapi/gnosis-safe-delegates-api-openapi.yml
- filename: gnosis-safe-messages-api-openapi.yml
  format: yaml
  label: Safe (Gnosis Safe) messages API
  slug: gnosis-safe-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gnosis-safe/refs/heads/main/openapi/gnosis-safe-messages-api-openapi.yml
- filename: gnosis-safe-modules-api-openapi.yml
  format: yaml
  label: Safe (Gnosis Safe) modules API
  slug: gnosis-safe-modules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gnosis-safe/refs/heads/main/openapi/gnosis-safe-modules-api-openapi.yml
- filename: gnosis-safe-owners-api-openapi.yml
  format: yaml
  label: Safe (Gnosis Safe) owners API
  slug: gnosis-safe-owners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gnosis-safe/refs/heads/main/openapi/gnosis-safe-owners-api-openapi.yml
- filename: gnosis-safe-safes-api-openapi.yml
  format: yaml
  label: Safe (Gnosis Safe) safes API
  slug: gnosis-safe-safes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gnosis-safe/refs/heads/main/openapi/gnosis-safe-safes-api-openapi.yml
- filename: gnosis-safe-tokens-api-openapi.yml
  format: yaml
  label: Safe (Gnosis Safe) tokens API
  slug: gnosis-safe-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gnosis-safe/refs/heads/main/openapi/gnosis-safe-tokens-api-openapi.yml
- filename: gnosis-safe-transactions-api-openapi.yml
  format: yaml
  label: Safe (Gnosis Safe) transactions API
  slug: gnosis-safe-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gnosis-safe/refs/heads/main/openapi/gnosis-safe-transactions-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Gnosis Safe Authentication
name_suffix: Authentication
oauth_flows: []
overview: Safe (Gnosis Safe) secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Safe (Gnosis Safe)
provider_slug: gnosis-safe
scheme_count: 2
schemes:
- in: cookie
  name: cookieAuth
  parameter: sessionid
  sources:
  - openapi/gnosis-safe-transaction-service-openapi.json
  type: apiKey
- description: Token-based authentication with required prefix "Token"
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/gnosis-safe-transaction-service-openapi.json
  type: apiKey
slug: gnosis-safe-authentication
source_filename: gnosis-safe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gnosis-safe-transaction-service-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: sessionid\n  sources:\n  - openapi/gnosis-safe-transaction-service-openapi.json\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Token-based authentication with required prefix \"Token\"\n  sources:\n  - openapi/gnosis-safe-transaction-service-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gnosis-safe/refs/heads/main/authentication/gnosis-safe-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Multisig
- Smart Contract
- Ethereum
- Web3
- Blockchain
- DeFi
- Safe
- Gnosis
- Wallets
---
