---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: coinmate-account-api-openapi.yml
  format: yaml
  label: Coinmate Account API
  slug: coinmate-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinmate/openapi/coinmate-account-api-openapi.yml
- filename: coinmate-bitcoin-api-openapi.yml
  format: yaml
  label: Coinmate Bitcoin API
  slug: coinmate-bitcoin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinmate/openapi/coinmate-bitcoin-api-openapi.yml
- filename: coinmate-cardano-api-openapi.yml
  format: yaml
  label: Coinmate Cardano API
  slug: coinmate-cardano-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinmate/openapi/coinmate-cardano-api-openapi.yml
- filename: coinmate-currencies-api-openapi.yml
  format: yaml
  label: Coinmate Currencies API
  slug: coinmate-currencies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinmate/openapi/coinmate-currencies-api-openapi.yml
- filename: coinmate-ethereum-api-openapi.yml
  format: yaml
  label: Coinmate Ethereum API
  slug: coinmate-ethereum-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinmate/openapi/coinmate-ethereum-api-openapi.yml
- filename: coinmate-fiat-api-openapi.yml
  format: yaml
  label: Coinmate FIAT API
  slug: coinmate-fiat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinmate/openapi/coinmate-fiat-api-openapi.yml
- filename: coinmate-history-api-openapi.yml
  format: yaml
  label: Coinmate History API
  slug: coinmate-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinmate/openapi/coinmate-history-api-openapi.yml
- filename: coinmate-litecoin-api-openapi.yml
  format: yaml
  label: Coinmate Litecoin API
  slug: coinmate-litecoin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinmate/openapi/coinmate-litecoin-api-openapi.yml
- filename: coinmate-market-data-api-openapi.yml
  format: yaml
  label: Coinmate Market Data API
  slug: coinmate-market-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinmate/openapi/coinmate-market-data-api-openapi.yml
- filename: coinmate-orders-api-openapi.yml
  format: yaml
  label: Coinmate Orders API
  slug: coinmate-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinmate/openapi/coinmate-orders-api-openapi.yml
- filename: coinmate-ripple-api-openapi.yml
  format: yaml
  label: Coinmate Ripple API
  slug: coinmate-ripple-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinmate/openapi/coinmate-ripple-api-openapi.yml
- filename: coinmate-solana-api-openapi.yml
  format: yaml
  label: Coinmate Solana API
  slug: coinmate-solana-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinmate/openapi/coinmate-solana-api-openapi.yml
- filename: coinmate-system-api-openapi.yml
  format: yaml
  label: Coinmate System API
  slug: coinmate-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinmate/openapi/coinmate-system-api-openapi.yml
- filename: coinmate-virtual-currency-api-openapi.yml
  format: yaml
  label: Coinmate Virtual Currency API
  slug: coinmate-virtual-currency-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinmate/openapi/coinmate-virtual-currency-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Coinmate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coinmate secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Coinmate
provider_slug: coinmate
scheme_count: 1
schemes:
- description: 'HMAC-SHA256 authentication. Requires the following headers:

    - `X-Coinmate-Client-ID` — your Client ID

    - `X-Coinmate-Nonce` — unique incrementing number

    - `X-Coinmate-Public-Key` — your API public key (optional)

    - `X-Coinmate-Signature` — `HMAC_SHA256(nonce + clientId + publicKey, privateKey)` uppercased hex


    Alternatively for POST endpoints, authentication can be provided via form parameters:

    `cli'
  in: header
  name: hmacAuth
  parameter: X-Coinmate-Signature
  sources:
  - openapi/coinmate-trading.yaml
  type: apiKey
slug: coinmate-authentication
source_filename: coinmate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: derived\nsource: openapi/coinmate-trading.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmacAuth\n  type: apiKey\n  in: header\n  parameter: X-Coinmate-Signature\n  description: |-\n    HMAC-SHA256 authentication. Requires the following headers:\n    - `X-Coinmate-Client-ID` — your Client ID\n    - `X-Coinmate-Nonce` — unique incrementing number\n    - `X-Coinmate-Public-Key` — your API public key (optional)\n    - `X-Coinmate-Signature` — `HMAC_SHA256(nonce + clientId + publicKey, privateKey)` uppercased hex\n\n    Alternatively for POST endpoints, authentication can be provided via form parameters:\n    `cli\n  sources:\n  - openapi/coinmate-trading.yaml\n"
source_yaml_url: https://artifacts.apis.io/coinmate/authentication/coinmate-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cryptocurrency Exchange
- Trading Platform
- Recurring Buy
- Premium Trading
- Czech Market
---
