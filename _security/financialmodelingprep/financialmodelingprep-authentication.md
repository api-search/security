---
api_key_in: []
api_specs:
- filename: financialmodelingprep-openapi.yml
  format: yaml
  label: Financial Modeling Prep Financial Statements API
  slug: financialmodelingprep-financial-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/financialmodelingprep/refs/heads/main/openapi/financialmodelingprep-openapi.yml
- filename: financialmodelingprep-openapi.yml
  format: yaml
  label: Financial Modeling Prep Quotes and Prices API
  slug: financialmodelingprep-quotes-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/financialmodelingprep/refs/heads/main/openapi/financialmodelingprep-openapi.yml
- filename: financialmodelingprep-openapi.yml
  format: yaml
  label: Financial Modeling Prep SEC Filings API
  slug: financialmodelingprep-sec-filings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/financialmodelingprep/refs/heads/main/openapi/financialmodelingprep-openapi.yml
- filename: financialmodelingprep-openapi.yml
  format: yaml
  label: Financial Modeling Prep Fundamentals API
  slug: financialmodelingprep-fundamentals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/financialmodelingprep/refs/heads/main/openapi/financialmodelingprep-openapi.yml
- filename: financialmodelingprep-openapi.yml
  format: yaml
  label: Financial Modeling Prep Analyst Estimates API
  slug: financialmodelingprep-analyst-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/financialmodelingprep/refs/heads/main/openapi/financialmodelingprep-openapi.yml
- filename: financialmodelingprep-openapi.yml
  format: yaml
  label: Financial Modeling Prep Economic Data API
  slug: financialmodelingprep-economic-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/financialmodelingprep/refs/heads/main/openapi/financialmodelingprep-openapi.yml
- filename: financialmodelingprep-asyncapi.yml
  format: yaml
  label: Financial Modeling Prep Real-Time WebSocket API
  slug: financialmodelingprep-realtime-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/financialmodelingprep/refs/heads/main/asyncapi/financialmodelingprep-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Financialmodelingprep Authentication
name_suffix: Authentication
oauth_flows: []
overview: Financial Modeling Prep secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Financial Modeling Prep
provider_slug: financialmodelingprep
scheme_count: 1
schemes:
- description: Every REST request is authenticated with an FMP API key passed as the `apikey` query parameter, e.g. ?apikey=YOUR_API_KEY. The same key authenticates the WebSocket streams via a login event carrying apiKey.
  in: query
  keyName: apikey
  name: apiKeyQuery
  sources:
  - openapi/financialmodelingprep-openapi.yml
  - https://site.financialmodelingprep.com/developer/docs/stable
  type: apiKey
slug: financialmodelingprep-authentication
source_filename: financialmodelingprep-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/financialmodelingprep-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  keyName: apikey\n  description: >-\n    Every REST request is authenticated with an FMP API key passed as the\n    `apikey` query parameter, e.g. ?apikey=YOUR_API_KEY. The same key\n    authenticates the WebSocket streams via a login event carrying apiKey.\n  sources:\n  - openapi/financialmodelingprep-openapi.yml\n  - https://site.financialmodelingprep.com/developer/docs/stable\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/financialmodelingprep/refs/heads/main/authentication/financialmodelingprep-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Financial Data
- Market Data
- Fundamentals
- SEC Filings
- Stocks
- Economic Indicators
- Quotes
- Regulatory Filings
---
