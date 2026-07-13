---
api_key_in: []
api_specs:
- filename: barchart-openapi.yml
  format: yaml
  label: Barchart Quotes API
  slug: barchart-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-openapi.yml
- filename: barchart-openapi.yml
  format: yaml
  label: Barchart History API
  slug: barchart-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-openapi.yml
- filename: barchart-openapi.yml
  format: yaml
  label: Barchart Reference & Equities API
  slug: barchart-reference-equities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-openapi.yml
- filename: barchart-openapi.yml
  format: yaml
  label: Barchart Futures & Options API
  slug: barchart-futures-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-openapi.yml
- filename: barchart-openapi.yml
  format: yaml
  label: Barchart Fundamentals API
  slug: barchart-fundamentals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-openapi.yml
- filename: barchart-openapi.yml
  format: yaml
  label: Barchart Corporate Actions & Earnings API
  slug: barchart-corporate-actions-earnings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-openapi.yml
- filename: barchart-openapi.yml
  format: yaml
  label: Barchart Cryptocurrency API
  slug: barchart-cryptocurrency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-openapi.yml
- filename: barchart-openapi.yml
  format: yaml
  label: Barchart Commodities & Agriculture API
  slug: barchart-commodities-agriculture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-openapi.yml
- filename: barchart-openapi.yml
  format: yaml
  label: Barchart Technicals & Charts API
  slug: barchart-technicals-charts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-openapi.yml
- filename: barchart-openapi.yml
  format: yaml
  label: Barchart News & Filings API
  slug: barchart-news-filings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-openapi.yml
- filename: barchart-openapi.yml
  format: yaml
  label: Barchart Weather API
  slug: barchart-weather-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: documented
name: Barchart Authentication
name_suffix: Authentication
oauth_flows: []
overview: Barchart secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Barchart
provider_slug: barchart
scheme_count: 1
schemes:
- description: Every Barchart OnDemand request carries an `apikey` query parameter (for example `?apikey=YOUR_API_KEY`). Keys are issued with a Barchart OnDemand subscription or enterprise agreement; a limited free trial key is available for evaluation. Real-time exchange data additionally requires exchange licensing.
  in: query
  keyName: apikey
  name: apiKeyQuery
  sources:
  - https://www.barchart.com/ondemand/api/getQuote
  - https://www.barchart.com/ondemand/faq
  type: apiKey
slug: barchart-authentication
source_filename: barchart-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: documented\nsource: https://www.barchart.com/ondemand/api + openapi/barchart-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  keyName: apikey\n  description: >-\n    Every Barchart OnDemand request carries an `apikey` query parameter (for\n    example `?apikey=YOUR_API_KEY`). Keys are issued with a Barchart OnDemand\n    subscription or enterprise agreement; a limited free trial key is available\n    for evaluation. Real-time exchange data additionally requires exchange\n    licensing.\n  sources:\n  - https://www.barchart.com/ondemand/api/getQuote\n  - https://www.barchart.com/ondemand/faq\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/authentication/barchart-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Market Data
- Financial Data
- Commodities
- Futures
- Options
- Reference Data
- Equities
- Historical Data
- Cryptocurrency
- Agriculture
---
