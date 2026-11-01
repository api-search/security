---
anonymous_access: false
api_key_in: []
api_specs:
- filename: roic-ai-bulk-downloads-api-openapi.yml
  format: yaml
  label: roic-ai Bulk Downloads API
  slug: roic-ai-bulk-downloads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roic-ai/openapi/roic-ai-bulk-downloads-api-openapi.yml
- filename: roic-ai-calendar-api-openapi.yml
  format: yaml
  label: roic-ai Calendar API
  slug: roic-ai-calendar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roic-ai/openapi/roic-ai-calendar-api-openapi.yml
- filename: roic-ai-company-api-openapi.yml
  format: yaml
  label: roic-ai Company API
  slug: roic-ai-company-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roic-ai/openapi/roic-ai-company-api-openapi.yml
- filename: roic-ai-company-events-api-openapi.yml
  format: yaml
  label: roic-ai Company Events API
  slug: roic-ai-company-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roic-ai/openapi/roic-ai-company-events-api-openapi.yml
- filename: roic-ai-content-api-openapi.yml
  format: yaml
  label: roic-ai Content API
  slug: roic-ai-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roic-ai/openapi/roic-ai-content-api-openapi.yml
- filename: roic-ai-countries-api-openapi.yml
  format: yaml
  label: roic-ai Countries API
  slug: roic-ai-countries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roic-ai/openapi/roic-ai-countries-api-openapi.yml
- filename: roic-ai-excel-api-openapi.yml
  format: yaml
  label: roic-ai Excel API
  slug: roic-ai-excel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roic-ai/openapi/roic-ai-excel-api-openapi.yml
- filename: roic-ai-exchanges-api-openapi.yml
  format: yaml
  label: roic-ai Exchanges API
  slug: roic-ai-exchanges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roic-ai/openapi/roic-ai-exchanges-api-openapi.yml
- filename: roic-ai-forex-api-openapi.yml
  format: yaml
  label: roic-ai Forex API
  slug: roic-ai-forex-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roic-ai/openapi/roic-ai-forex-api-openapi.yml
- filename: roic-ai-fundamental-api-openapi.yml
  format: yaml
  label: roic-ai Fundamental API
  slug: roic-ai-fundamental-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roic-ai/openapi/roic-ai-fundamental-api-openapi.yml
- filename: roic-ai-fundamentals-api-openapi.yml
  format: yaml
  label: roic-ai Fundamentals API
  slug: roic-ai-fundamentals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roic-ai/openapi/roic-ai-fundamentals-api-openapi.yml
- filename: roic-ai-industries-api-openapi.yml
  format: yaml
  label: roic-ai Industries API
  slug: roic-ai-industries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roic-ai/openapi/roic-ai-industries-api-openapi.yml
- filename: roic-ai-market-data-api-openapi.yml
  format: yaml
  label: roic-ai Market Data API
  slug: roic-ai-market-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roic-ai/openapi/roic-ai-market-data-api-openapi.yml
- filename: roic-ai-reference-data-api-openapi.yml
  format: yaml
  label: roic-ai Reference Data API
  slug: roic-ai-reference-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roic-ai/openapi/roic-ai-reference-data-api-openapi.yml
- filename: roic-ai-sectors-api-openapi.yml
  format: yaml
  label: roic-ai Sectors API
  slug: roic-ai-sectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roic-ai/openapi/roic-ai-sectors-api-openapi.yml
- filename: roic-ai-stock-prices-api-openapi.yml
  format: yaml
  label: roic-ai Stock Prices API
  slug: roic-ai-stock-prices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roic-ai/openapi/roic-ai-stock-prices-api-openapi.yml
- filename: roic-ai-stock-splits-api-openapi.yml
  format: yaml
  label: roic-ai Stock Splits API
  slug: roic-ai-stock-splits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roic-ai/openapi/roic-ai-stock-splits-api-openapi.yml
- filename: roic-ai-tickers-api-openapi.yml
  format: yaml
  label: roic-ai Tickers API
  slug: roic-ai-tickers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roic-ai/openapi/roic-ai-tickers-api-openapi.yml
- filename: roic-ai-usage-api-openapi.yml
  format: yaml
  label: roic-ai Usage API
  slug: roic-ai-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roic-ai/openapi/roic-ai-usage-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Roic Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: roic-ai declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: roic-ai
provider_slug: roic-ai
scheme_count: 2
schemes:
- description: API key passed as query parameter "apikey"
  in: query
  name: apikey
  type: apiKey
- bearerFormat: JWT
  description: API key passed in Authorization header as Bearer token
  scheme: bearer
  type: http
slug: roic-ai-authentication
source_filename: roic-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://www.roic.ai/api/docs/authentication\nschemes:\n  - type: apiKey\n    name: apikey\n    in: query\n    description: API key passed as query parameter \"apikey\"\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: API key passed in Authorization header as Bearer token\n"
source_yaml_url: https://artifacts.apis.io/roic-ai/authentication/roic-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Finance
- Data
- API
- Stock
---
