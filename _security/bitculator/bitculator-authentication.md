---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bitculator-alarms-api-openapi.yml
  format: yaml
  label: Bitculator Alarms API
  slug: bitculator-alarms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitculator/refs/heads/main/openapi/bitculator-alarms-api-openapi.yml
- filename: bitculator-calculators-api-openapi.yml
  format: yaml
  label: Bitculator Calculators API
  slug: bitculator-calculators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitculator/refs/heads/main/openapi/bitculator-calculators-api-openapi.yml
- filename: bitculator-coins-api-openapi.yml
  format: yaml
  label: Bitculator Coins API
  slug: bitculator-coins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitculator/refs/heads/main/openapi/bitculator-coins-api-openapi.yml
- filename: bitculator-conversion-api-openapi.yml
  format: yaml
  label: Bitculator Conversion API
  slug: bitculator-conversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitculator/refs/heads/main/openapi/bitculator-conversion-api-openapi.yml
- filename: bitculator-editorial-api-openapi.yml
  format: yaml
  label: Bitculator Editorial API
  slug: bitculator-editorial-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitculator/refs/heads/main/openapi/bitculator-editorial-api-openapi.yml
- filename: bitculator-exchanges-api-openapi.yml
  format: yaml
  label: Bitculator Exchanges API
  slug: bitculator-exchanges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitculator/refs/heads/main/openapi/bitculator-exchanges-api-openapi.yml
- filename: bitculator-global-market-api-openapi.yml
  format: yaml
  label: Bitculator Global Market API
  slug: bitculator-global-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitculator/refs/heads/main/openapi/bitculator-global-market-api-openapi.yml
- filename: bitculator-indicators-api-openapi.yml
  format: yaml
  label: Bitculator Indicators API
  slug: bitculator-indicators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitculator/refs/heads/main/openapi/bitculator-indicators-api-openapi.yml
- filename: bitculator-liquidations-api-openapi.yml
  format: yaml
  label: Bitculator Liquidations API
  slug: bitculator-liquidations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitculator/refs/heads/main/openapi/bitculator-liquidations-api-openapi.yml
- filename: bitculator-markets-api-openapi.yml
  format: yaml
  label: Bitculator Markets API
  slug: bitculator-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitculator/refs/heads/main/openapi/bitculator-markets-api-openapi.yml
- filename: bitculator-meta-api-openapi.yml
  format: yaml
  label: Bitculator Meta API
  slug: bitculator-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitculator/refs/heads/main/openapi/bitculator-meta-api-openapi.yml
- filename: bitculator-prices-api-openapi.yml
  format: yaml
  label: Bitculator Prices API
  slug: bitculator-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitculator/refs/heads/main/openapi/bitculator-prices-api-openapi.yml
- filename: bitculator-sentiment-api-openapi.yml
  format: yaml
  label: Bitculator Sentiment API
  slug: bitculator-sentiment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitculator/refs/heads/main/openapi/bitculator-sentiment-api-openapi.yml
- filename: bitculator-wallets-api-openapi.yml
  format: yaml
  label: Bitculator Wallets API
  slug: bitculator-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitculator/refs/heads/main/openapi/bitculator-wallets-api-openapi.yml
- filename: bitculator-webhooks-api-openapi.yml
  format: yaml
  label: Bitculator Webhooks API
  slug: bitculator-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitculator/refs/heads/main/openapi/bitculator-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Bitculator Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bitculator secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bitculator
provider_slug: bitculator
scheme_count: 1
schemes:
- description: Create a Data API key in your <a href="/user/developer/api">developer console</a> — keys are Bearer-only and carry the <code>data-api</code> ability. Keep them server-side; they are never meant for client-side embedding.
  name: default
  scheme: bearer
  sources:
  - openapi/bitculator-data-api-openapi.json
  type: http
slug: bitculator-authentication
source_filename: bitculator-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: derived\nsource: openapi/bitculator-data-api-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: default\n  type: http\n  scheme: bearer\n  description: Create a Data API key in your <a href=\"/user/developer/api\">developer console</a>\n    — keys are Bearer-only and carry the <code>data-api</code> ability. Keep them server-side;\n    they are never meant for client-side embedding.\n  sources:\n  - openapi/bitculator-data-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitculator/refs/heads/main/authentication/bitculator-authentication.yml
summary_line: http · 1 scheme
tags:
- Cryptocurrency
- crypto-market-data
- Blockchain
- Finance
- Fintech
- Web3
- Trading
- Exchange Data
- Wallets
- Sentiment
- Indicators
---
