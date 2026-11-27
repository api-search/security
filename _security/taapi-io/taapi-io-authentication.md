---
anonymous_access: false
api_key_in: []
api_specs:
- filename: taapi-io-cycle-api-openapi.yml
  format: yaml
  label: TAAPI.IO Cycle API
  slug: taapi-io-cycle-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taapi-io/openapi/taapi-io-cycle-api-openapi.yml
- filename: taapi-io-divergence-api-openapi.yml
  format: yaml
  label: TAAPI.IO Divergence API
  slug: taapi-io-divergence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taapi-io/openapi/taapi-io-divergence-api-openapi.yml
- filename: taapi-io-indicator-calls-api-openapi.yml
  format: yaml
  label: TAAPI.IO Indicator Calls API
  slug: taapi-io-indicator-calls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taapi-io/openapi/taapi-io-indicator-calls-api-openapi.yml
- filename: taapi-io-manual-candles-api-openapi.yml
  format: yaml
  label: TAAPI.IO Manual Candles API
  slug: taapi-io-manual-candles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taapi-io/openapi/taapi-io-manual-candles-api-openapi.yml
- filename: taapi-io-market-data-api-openapi.yml
  format: yaml
  label: TAAPI.IO Market Data API
  slug: taapi-io-market-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taapi-io/openapi/taapi-io-market-data-api-openapi.yml
- filename: taapi-io-market-structure-api-openapi.yml
  format: yaml
  label: TAAPI.IO Market Structure API
  slug: taapi-io-market-structure-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taapi-io/openapi/taapi-io-market-structure-api-openapi.yml
- filename: taapi-io-math-api-openapi.yml
  format: yaml
  label: TAAPI.IO Math API
  slug: taapi-io-math-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taapi-io/openapi/taapi-io-math-api-openapi.yml
- filename: taapi-io-momentum-api-openapi.yml
  format: yaml
  label: TAAPI.IO Momentum API
  slug: taapi-io-momentum-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taapi-io/openapi/taapi-io-momentum-api-openapi.yml
- filename: taapi-io-pattern-recognition-advanced-api-openapi.yml
  format: yaml
  label: TAAPI.IO Pattern Recognition - Advanced API
  slug: taapi-io-pattern-recognition-advanced-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taapi-io/openapi/taapi-io-pattern-recognition-advanced-api-openapi.yml
- filename: taapi-io-pattern-recognition-simple-api-openapi.yml
  format: yaml
  label: TAAPI.IO Pattern Recognition - Simple API
  slug: taapi-io-pattern-recognition-simple-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taapi-io/openapi/taapi-io-pattern-recognition-simple-api-openapi.yml
- filename: taapi-io-reference-data-api-openapi.yml
  format: yaml
  label: TAAPI.IO Reference Data API
  slug: taapi-io-reference-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taapi-io/openapi/taapi-io-reference-data-api-openapi.yml
- filename: taapi-io-statistics-api-openapi.yml
  format: yaml
  label: TAAPI.IO Statistics API
  slug: taapi-io-statistics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taapi-io/openapi/taapi-io-statistics-api-openapi.yml
- filename: taapi-io-trend-api-openapi.yml
  format: yaml
  label: TAAPI.IO Trend API
  slug: taapi-io-trend-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taapi-io/openapi/taapi-io-trend-api-openapi.yml
- filename: taapi-io-volatility-api-openapi.yml
  format: yaml
  label: TAAPI.IO Volatility API
  slug: taapi-io-volatility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taapi-io/openapi/taapi-io-volatility-api-openapi.yml
- filename: taapi-io-volume-api-openapi.yml
  format: yaml
  label: TAAPI.IO Volume API
  slug: taapi-io-volume-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taapi-io/openapi/taapi-io-volume-api-openapi.yml
auth_types: []
description: Authentication schemes as published on the TAAPI.IO documentation page.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: TAAPI.IO Authentication
name_suffix: Authentication
oauth_flows: []
overview: TAAPI.IO declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: TAAPI.IO
provider_slug: taapi-io
scheme_count: 1
schemes:
- evidence: 'Every request requires a Authorization: Bearer <key> header.'
  header: Authorization
  how_to_obtain: Sign up at taapi.io and copy your v2 API key (the Production key, starting with taapi_live_sk_) from API Keys in the dashboard at app.taapi.io.
  location: header
  name: Bearer
  type: http-bearer
slug: taapi-io-authentication
source_filename: taapi-io-authentication.yml
source_heading: Authentication Profile
source_url: https://taapi.io/documentation/
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://taapi.io/documentation/\nsources:\n- https://taapi.io/documentation/\ndescription: Authentication schemes as published on the TAAPI.IO documentation page.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Every request requires a Authorization: Bearer <key> header.'\n  location: header\n  header: Authorization\n  how_to_obtain: Sign up at taapi.io and copy your v2 API key (the Production key, starting with taapi_live_sk_) from API Keys in the dashboard\n    at app.taapi.io.\ndocs: https://taapi.io/documentation/\n"
source_yaml_url: https://artifacts.apis.io/taapi-io/authentication/taapi-io-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Finance
- Cryptocurrency
- Technical Analysis
---
