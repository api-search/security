---
anonymous_access: false
api_key_in: []
api_specs:
- filename: barchart-charts-and-analytics-api-openapi.yml
  format: yaml
  label: Barchart Charts and Analytics API
  slug: barchart-charts-and-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-charts-and-analytics-api-openapi.yml
- filename: barchart-cryptocurrency-data-api-openapi.yml
  format: yaml
  label: Barchart Cryptocurrency Data API
  slug: barchart-cryptocurrency-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-cryptocurrency-data-api-openapi.yml
- filename: barchart-leaderboards-and-lists-api-openapi.yml
  format: yaml
  label: Barchart Leaderboards and Lists API
  slug: barchart-leaderboards-and-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-leaderboards-and-lists-api-openapi.yml
- filename: barchart-metadata-api-openapi.yml
  format: yaml
  label: Barchart Metadata API
  slug: barchart-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-metadata-api-openapi.yml
- filename: barchart-news-and-filings-api-openapi.yml
  format: yaml
  label: Barchart News and Filings API
  slug: barchart-news-and-filings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-news-and-filings-api-openapi.yml
- filename: barchart-other-data-api-openapi.yml
  format: yaml
  label: Barchart Other Data API
  slug: barchart-other-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-other-data-api-openapi.yml
- filename: barchart-price-data-api-openapi.yml
  format: yaml
  label: Barchart Price Data API
  slug: barchart-price-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-price-data-api-openapi.yml
- filename: barchart-profiles-and-financial-data-api-openapi.yml
  format: yaml
  label: Barchart Profiles and Financial Data API
  slug: barchart-profiles-and-financial-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-profiles-and-financial-data-api-openapi.yml
- filename: barchart-splits-dividends-and-earnings-api-openapi.yml
  format: yaml
  label: Barchart Splits, Dividends, and Earnings API
  slug: barchart-splits-dividends-and-earnings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-splits-dividends-and-earnings-api-openapi.yml
- filename: barchart-etfs-api-openapi.yml
  format: yaml
  label: Barchart ET Fs API
  slug: barchart-etfs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barchart/refs/heads/main/openapi/barchart-etfs-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
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
- Stocks
- Historical Data
- Cryptocurrency
- Agriculture
---
