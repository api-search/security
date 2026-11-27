---
anonymous_access: false
api_key_in: []
api_specs:
- filename: coinrithm-com-futures-api-openapi.yml
  format: yaml
  label: CoinRithm Futures API
  slug: coinrithm-com-futures-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinrithm-com/openapi/coinrithm-com-futures-api-openapi.yml
- filename: coinrithm-com-identity-api-openapi.yml
  format: yaml
  label: CoinRithm Identity API
  slug: coinrithm-com-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinrithm-com/openapi/coinrithm-com-identity-api-openapi.yml
- filename: coinrithm-com-ledger-api-openapi.yml
  format: yaml
  label: CoinRithm Ledger API
  slug: coinrithm-com-ledger-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinrithm-com/openapi/coinrithm-com-ledger-api-openapi.yml
- filename: coinrithm-com-prediction-markets-api-openapi.yml
  format: yaml
  label: CoinRithm Prediction Markets API
  slug: coinrithm-com-prediction-markets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinrithm-com/openapi/coinrithm-com-prediction-markets-api-openapi.yml
- filename: coinrithm-com-public-crypto-data-api-openapi.yml
  format: yaml
  label: CoinRithm Public Crypto Data API
  slug: coinrithm-com-public-crypto-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinrithm-com/openapi/coinrithm-com-public-crypto-data-api-openapi.yml
- filename: coinrithm-com-public-market-data-api-openapi.yml
  format: yaml
  label: CoinRithm Public Market Data API
  slug: coinrithm-com-public-market-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinrithm-com/openapi/coinrithm-com-public-market-data-api-openapi.yml
- filename: coinrithm-com-public-pm-data-api-openapi.yml
  format: yaml
  label: CoinRithm Public Pm Data API
  slug: coinrithm-com-public-pm-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinrithm-com/openapi/coinrithm-com-public-pm-data-api-openapi.yml
- filename: coinrithm-com-reads-api-openapi.yml
  format: yaml
  label: CoinRithm Reads API
  slug: coinrithm-com-reads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinrithm-com/openapi/coinrithm-com-reads-api-openapi.yml
- filename: coinrithm-com-spot-api-openapi.yml
  format: yaml
  label: CoinRithm Spot API
  slug: coinrithm-com-spot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinrithm-com/openapi/coinrithm-com-spot-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: CoinRithm Authentication
name_suffix: Authentication
oauth_flows: []
overview: CoinRithm secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CoinRithm
provider_slug: coinrithm-com
scheme_count: 1
schemes:
- description: Personal CoinRithm API key, format `crk_live_…`.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/coinrithm-com-openapi.yml
  type: http
slug: coinrithm-com-authentication
source_filename: coinrithm-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/coinrithm-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Personal CoinRithm API key, format `crk_live_…`.\n  sources:\n  - openapi/coinrithm-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/coinrithm-com/authentication/coinrithm-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Prediction Markets
- Crypto Prices
- Paper Trading
- Agentic Trading
- Research Service
- Live Market Data
---
