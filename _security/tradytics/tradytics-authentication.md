---
anonymous_access: false
api_key_in: []
api_specs:
- filename: tradytics-ai-fund-api-openapi.yml
  format: yaml
  label: Tradytics AI Fund API
  slug: tradytics-ai-fund-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradytics/openapi/tradytics-ai-fund-api-openapi.yml
- filename: tradytics-calendar-and-news-api-openapi.yml
  format: yaml
  label: Tradytics Calendar and news API
  slug: tradytics-calendar-and-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradytics/openapi/tradytics-calendar-and-news-api-openapi.yml
- filename: tradytics-dark-pool-api-openapi.yml
  format: yaml
  label: Tradytics Dark pool API
  slug: tradytics-dark-pool-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradytics/openapi/tradytics-dark-pool-api-openapi.yml
- filename: tradytics-dealer-positioning-api-openapi.yml
  format: yaml
  label: Tradytics Dealer positioning API
  slug: tradytics-dealer-positioning-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradytics/openapi/tradytics-dealer-positioning-api-openapi.yml
- filename: tradytics-disclosures-api-openapi.yml
  format: yaml
  label: Tradytics Disclosures API
  slug: tradytics-disclosures-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradytics/openapi/tradytics-disclosures-api-openapi.yml
- filename: tradytics-filings-api-openapi.yml
  format: yaml
  label: Tradytics Filings API
  slug: tradytics-filings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradytics/openapi/tradytics-filings-api-openapi.yml
- filename: tradytics-fundamentals-api-openapi.yml
  format: yaml
  label: Tradytics Fundamentals API
  slug: tradytics-fundamentals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradytics/openapi/tradytics-fundamentals-api-openapi.yml
- filename: tradytics-insights-api-openapi.yml
  format: yaml
  label: Tradytics Insights API
  slug: tradytics-insights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradytics/openapi/tradytics-insights-api-openapi.yml
- filename: tradytics-kpis-api-openapi.yml
  format: yaml
  label: Tradytics KPIs API
  slug: tradytics-kpis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradytics/openapi/tradytics-kpis-api-openapi.yml
- filename: tradytics-market-api-openapi.yml
  format: yaml
  label: Tradytics Market API
  slug: tradytics-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradytics/openapi/tradytics-market-api-openapi.yml
- filename: tradytics-options-contracts-api-openapi.yml
  format: yaml
  label: Tradytics Options contracts API
  slug: tradytics-options-contracts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradytics/openapi/tradytics-options-contracts-api-openapi.yml
- filename: tradytics-options-flow-api-openapi.yml
  format: yaml
  label: Tradytics Options flow API
  slug: tradytics-options-flow-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradytics/openapi/tradytics-options-flow-api-openapi.yml
- filename: tradytics-probabilities-api-openapi.yml
  format: yaml
  label: Tradytics Probabilities API
  slug: tradytics-probabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradytics/openapi/tradytics-probabilities-api-openapi.yml
- filename: tradytics-screener-api-openapi.yml
  format: yaml
  label: Tradytics Screener API
  slug: tradytics-screener-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradytics/openapi/tradytics-screener-api-openapi.yml
- filename: tradytics-signals-api-openapi.yml
  format: yaml
  label: Tradytics Signals API
  slug: tradytics-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradytics/openapi/tradytics-signals-api-openapi.yml
- filename: tradytics-stocks-api-openapi.yml
  format: yaml
  label: Tradytics Stocks API
  slug: tradytics-stocks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradytics/openapi/tradytics-stocks-api-openapi.yml
- filename: tradytics-symbols-api-openapi.yml
  format: yaml
  label: Tradytics Symbols API
  slug: tradytics-symbols-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradytics/openapi/tradytics-symbols-api-openapi.yml
- filename: tradytics-volatility-api-openapi.yml
  format: yaml
  label: Tradytics Volatility API
  slug: tradytics-volatility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradytics/openapi/tradytics-volatility-api-openapi.yml
- filename: tradytics-your-account-api-openapi.yml
  format: yaml
  label: Tradytics Your account API
  slug: tradytics-your-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tradytics/openapi/tradytics-your-account-api-openapi.yml
auth_types: []
description: Authentication schemes for Tradytics API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Tradytics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tradytics declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Tradytics
provider_slug: tradytics
scheme_count: 1
schemes:
- evidence: Send your API key in the URL as the apiKey query parameter.
  how_to_obtain: Your key is on the API keys page, readable any time.
  location: query
  name: apiKey
  type: apiKey
slug: tradytics-authentication
source_filename: tradytics-authentication.yml
source_heading: Authentication Profile
source_url: https://tradytics.com/docs/authentication
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://tradytics.com/docs/authentication\nsources:\n- https://tradytics.com/docs/authentication\n- https://tradytics.com/developer/keys\n- https://tradytics.com/docs/quickstart\n- https://tradytics.com/docs/quickstart#create-a-key\ndescription: Authentication schemes for Tradytics API\nschemes:\n- type: apiKey\n  name: apiKey\n  evidence: Send your API key in the URL as the apiKey query parameter.\n  location: query\n  how_to_obtain: Your key is on the API keys page, readable any time.\ndocs: https://tradytics.com/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/tradytics/authentication/tradytics-authentication.yml
summary_line: 1 scheme
tags:
- Options
- Dark pool
- Artificial Intelligence
- Market Data
- Analytics
---
