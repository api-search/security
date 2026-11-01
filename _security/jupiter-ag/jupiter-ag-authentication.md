---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: jupiter-ag-events-api-openapi.yml
  format: yaml
  label: Jupiter Events API
  slug: jupiter-ag-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiter-ag/openapi/jupiter-ag-events-api-openapi.yml
- filename: jupiter-ag-forecast-api-openapi.yml
  format: yaml
  label: Jupiter Forecast API
  slug: jupiter-ag-forecast-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiter-ag/openapi/jupiter-ag-forecast-api-openapi.yml
- filename: jupiter-ag-history-api-openapi.yml
  format: yaml
  label: Jupiter History API
  slug: jupiter-ag-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiter-ag/openapi/jupiter-ag-history-api-openapi.yml
- filename: jupiter-ag-leaderboards-api-openapi.yml
  format: yaml
  label: Jupiter Leaderboards API
  slug: jupiter-ag-leaderboards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiter-ag/openapi/jupiter-ag-leaderboards-api-openapi.yml
- filename: jupiter-ag-markets-api-openapi.yml
  format: yaml
  label: Jupiter Markets API
  slug: jupiter-ag-markets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiter-ag/openapi/jupiter-ag-markets-api-openapi.yml
- filename: jupiter-ag-orderbook-api-openapi.yml
  format: yaml
  label: Jupiter Orderbook API
  slug: jupiter-ag-orderbook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiter-ag/openapi/jupiter-ag-orderbook-api-openapi.yml
- filename: jupiter-ag-orders-api-openapi.yml
  format: yaml
  label: Jupiter Orders API
  slug: jupiter-ag-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiter-ag/openapi/jupiter-ag-orders-api-openapi.yml
- filename: jupiter-ag-positions-api-openapi.yml
  format: yaml
  label: Jupiter Positions API
  slug: jupiter-ag-positions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiter-ag/openapi/jupiter-ag-positions-api-openapi.yml
- filename: jupiter-ag-profile-api-openapi.yml
  format: yaml
  label: Jupiter Profile API
  slug: jupiter-ag-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiter-ag/openapi/jupiter-ag-profile-api-openapi.yml
- filename: jupiter-ag-trades-api-openapi.yml
  format: yaml
  label: Jupiter Trades API
  slug: jupiter-ag-trades-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiter-ag/openapi/jupiter-ag-trades-api-openapi.yml
- filename: jupiter-ag-trading-api-openapi.yml
  format: yaml
  label: Jupiter Trading API
  slug: jupiter-ag-trading-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiter-ag/openapi/jupiter-ag-trading-api-openapi.yml
- filename: jupiter-ag-vault-api-openapi.yml
  format: yaml
  label: Jupiter Vault API
  slug: jupiter-ag-vault-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiter-ag/openapi/jupiter-ag-vault-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Jupiter Ag Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jupiter secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Jupiter
provider_slug: jupiter-ag
scheme_count: 1
schemes:
- description: Jupiter API key issued via the Jupiter Developer Platform.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/jupiter-ag-openapi.yml
  type: apiKey
slug: jupiter-ag-authentication
source_filename: jupiter-ag-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/jupiter-ag-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Jupiter API key issued via the Jupiter Developer Platform.\n  sources:\n  - openapi/jupiter-ag-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/jupiter-ag/authentication/jupiter-ag-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Solana
- DeFi
- DEX Aggregator
- Swap
- Perpetuals
- Limit Orders
- DCA
- Lending
---
