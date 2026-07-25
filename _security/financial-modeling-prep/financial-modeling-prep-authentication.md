---
api_key_in:
- query
- header
api_specs:
- filename: financial-modeling-prep-balance-sheet-statement-api-openapi.yml
  format: yaml
  label: Financial Modeling Prep Balance Sheet Statement API
  slug: financial-modeling-prep-balance-sheet-statement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/financial-modeling-prep/refs/heads/main/openapi/financial-modeling-prep-balance-sheet-statement-api-openapi.yml
- filename: financial-modeling-prep-cash-flow-statement-api-openapi.yml
  format: yaml
  label: Financial Modeling Prep Cash Flow Statement API
  slug: financial-modeling-prep-cash-flow-statement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/financial-modeling-prep/refs/heads/main/openapi/financial-modeling-prep-cash-flow-statement-api-openapi.yml
- filename: financial-modeling-prep-historical-price-full-api-openapi.yml
  format: yaml
  label: Financial Modeling Prep Historical Price Full API
  slug: financial-modeling-prep-historical-price-full-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/financial-modeling-prep/refs/heads/main/openapi/financial-modeling-prep-historical-price-full-api-openapi.yml
- filename: financial-modeling-prep-income-statement-api-openapi.yml
  format: yaml
  label: Financial Modeling Prep Income Statement API
  slug: financial-modeling-prep-income-statement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/financial-modeling-prep/refs/heads/main/openapi/financial-modeling-prep-income-statement-api-openapi.yml
- filename: financial-modeling-prep-insider-trading-api-openapi.yml
  format: yaml
  label: Financial Modeling Prep Insider Trading API
  slug: financial-modeling-prep-insider-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/financial-modeling-prep/refs/heads/main/openapi/financial-modeling-prep-insider-trading-api-openapi.yml
- filename: financial-modeling-prep-profile-api-openapi.yml
  format: yaml
  label: Financial Modeling Prep Profile API
  slug: financial-modeling-prep-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/financial-modeling-prep/refs/heads/main/openapi/financial-modeling-prep-profile-api-openapi.yml
- filename: financial-modeling-prep-quote-api-openapi.yml
  format: yaml
  label: Financial Modeling Prep Quote API
  slug: financial-modeling-prep-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/financial-modeling-prep/refs/heads/main/openapi/financial-modeling-prep-quote-api-openapi.yml
- filename: financial-modeling-prep-ratios-api-openapi.yml
  format: yaml
  label: Financial Modeling Prep Ratios API
  slug: financial-modeling-prep-ratios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/financial-modeling-prep/refs/heads/main/openapi/financial-modeling-prep-ratios-api-openapi.yml
- filename: financial-modeling-prep-search-api-openapi.yml
  format: yaml
  label: Financial Modeling Prep Search API
  slug: financial-modeling-prep-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/financial-modeling-prep/refs/heads/main/openapi/financial-modeling-prep-search-api-openapi.yml
- filename: financial-modeling-prep-stock-api-openapi.yml
  format: yaml
  label: Financial Modeling Prep Stock API
  slug: financial-modeling-prep-stock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/financial-modeling-prep/refs/heads/main/openapi/financial-modeling-prep-stock-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Financial Modeling Prep Authentication
name_suffix: Authentication
oauth_flows: []
overview: Financial Modeling Prep secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Financial Modeling Prep
provider_slug: financial-modeling-prep
scheme_count: 2
schemes:
- in: query
  name: apiKeyQuery
  notes: Append ?apikey=YOUR_API_KEY to every request; use &apikey= when other query parameters exist.
  parameter: apikey
  sources:
  - openapi/financial-modeling-prep-quote-api-openapi.yml
  type: apiKey
- in: header
  name: apiKeyHeader
  notes: 'Alternatively include the API key in the request header as apikey: YOUR_API_KEY.'
  parameter: apikey
  sources:
  - openapi/financial-modeling-prep-quote-api-openapi.yml
  type: apiKey
slug: financial-modeling-prep-authentication
source_filename: financial-modeling-prep-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: openapi/ securitySchemes + https://site.financialmodelingprep.com/api-docs.md\ndocs: https://site.financialmodelingprep.com/developer/docs\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\n  - header\n  oauth2_flows: []\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: apikey\n  notes: Append ?apikey=YOUR_API_KEY to every request; use &apikey= when other query parameters exist.\n  sources:\n  - openapi/financial-modeling-prep-quote-api-openapi.yml\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: apikey\n  notes: 'Alternatively include the API key in the request header as apikey: YOUR_API_KEY.'\n  sources:\n  - openapi/financial-modeling-prep-quote-api-openapi.yml\nnotes: API keys are issued on signup (https://site.financialmodelingprep.com/register). The platform publishes RFC\n  8414 OAuth authorization-server metadata at /.well-known/oauth-authorization-server, but OAuth is\
  \ not a documented\n  authentication method for the market-data API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/financial-modeling-prep/refs/heads/main/authentication/financial-modeling-prep-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Financial Data
- Market Data
- Stocks
- Quotes
- Fundamentals
- Financial Statements
- Historical
---
