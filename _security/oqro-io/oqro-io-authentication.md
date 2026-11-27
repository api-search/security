---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: oqro-io-baskets-api-openapi.yml
  format: yaml
  label: OQRO Baskets API
  slug: oqro-io-baskets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oqro-io/openapi/oqro-io-baskets-api-openapi.yml
- filename: oqro-io-calendar-api-openapi.yml
  format: yaml
  label: OQRO Calendar API
  slug: oqro-io-calendar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oqro-io/openapi/oqro-io-calendar-api-openapi.yml
- filename: oqro-io-companies-api-openapi.yml
  format: yaml
  label: OQRO Companies API
  slug: oqro-io-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oqro-io/openapi/oqro-io-companies-api-openapi.yml
- filename: oqro-io-compare-api-openapi.yml
  format: yaml
  label: OQRO Compare API
  slug: oqro-io-compare-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oqro-io/openapi/oqro-io-compare-api-openapi.yml
- filename: oqro-io-congress-trades-api-openapi.yml
  format: yaml
  label: OQRO Congress Trades API
  slug: oqro-io-congress-trades-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oqro-io/openapi/oqro-io-congress-trades-api-openapi.yml
- filename: oqro-io-contracts-api-openapi.yml
  format: yaml
  label: OQRO Contracts API
  slug: oqro-io-contracts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oqro-io/openapi/oqro-io-contracts-api-openapi.yml
- filename: oqro-io-economy-api-openapi.yml
  format: yaml
  label: OQRO Economy API
  slug: oqro-io-economy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oqro-io/openapi/oqro-io-economy-api-openapi.yml
- filename: oqro-io-fund-moves-api-openapi.yml
  format: yaml
  label: OQRO Fund Moves API
  slug: oqro-io-fund-moves-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oqro-io/openapi/oqro-io-fund-moves-api-openapi.yml
- filename: oqro-io-insider-trades-api-openapi.yml
  format: yaml
  label: OQRO Insider Trades API
  slug: oqro-io-insider-trades-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oqro-io/openapi/oqro-io-insider-trades-api-openapi.yml
- filename: oqro-io-leaderboard-api-openapi.yml
  format: yaml
  label: OQRO Leaderboard API
  slug: oqro-io-leaderboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oqro-io/openapi/oqro-io-leaderboard-api-openapi.yml
- filename: oqro-io-lobbying-api-openapi.yml
  format: yaml
  label: OQRO Lobbying API
  slug: oqro-io-lobbying-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oqro-io/openapi/oqro-io-lobbying-api-openapi.yml
- filename: oqro-io-prices-api-openapi.yml
  format: yaml
  label: OQRO Prices API
  slug: oqro-io-prices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oqro-io/openapi/oqro-io-prices-api-openapi.yml
- filename: oqro-io-rankings-api-openapi.yml
  format: yaml
  label: OQRO Rankings API
  slug: oqro-io-rankings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oqro-io/openapi/oqro-io-rankings-api-openapi.yml
- filename: oqro-io-screen-api-openapi.yml
  format: yaml
  label: OQRO Screen API
  slug: oqro-io-screen-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oqro-io/openapi/oqro-io-screen-api-openapi.yml
- filename: oqro-io-stats-api-openapi.yml
  format: yaml
  label: OQRO Stats API
  slug: oqro-io-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oqro-io/openapi/oqro-io-stats-api-openapi.yml
- filename: oqro-io-votes-near-trades-api-openapi.yml
  format: yaml
  label: OQRO Votes Near Trades API
  slug: oqro-io-votes-near-trades-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oqro-io/openapi/oqro-io-votes-near-trades-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: OQRO Authentication
name_suffix: Authentication
oauth_flows: []
overview: OQRO secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: OQRO
provider_slug: oqro-io
scheme_count: 2
schemes:
- name: bearer
  scheme: bearer
  sources:
  - openapi/oqro-io-openapi.json
  type: http
- in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/oqro-io-openapi.json
  type: apiKey
slug: oqro-io-authentication
source_filename: oqro-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: derived\nsource: openapi/oqro-io-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/oqro-io-openapi.json\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/oqro-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/oqro-io/authentication/oqro-io-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Insider Trades
- Politician Trades
- Fund Moves
- Federal Contracts
- Mergers and Acquisitions
- Financial Data API
- US public filings
---
