---
api_key_in:
- query
api_specs:
- filename: marketstack-bonds-api-openapi.yml
  format: yaml
  label: Marketstack Bonds API
  slug: marketstack-bonds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketstack/refs/heads/main/openapi/marketstack-bonds-api-openapi.yml
- filename: marketstack-commodities-api-openapi.yml
  format: yaml
  label: Marketstack Commodities API
  slug: marketstack-commodities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketstack/refs/heads/main/openapi/marketstack-commodities-api-openapi.yml
- filename: marketstack-company-ratings-api-openapi.yml
  format: yaml
  label: Marketstack Company Ratings API
  slug: marketstack-company-ratings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketstack/refs/heads/main/openapi/marketstack-company-ratings-api-openapi.yml
- filename: marketstack-currencies-api-openapi.yml
  format: yaml
  label: Marketstack Currencies API
  slug: marketstack-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketstack/refs/heads/main/openapi/marketstack-currencies-api-openapi.yml
- filename: marketstack-dividends-api-openapi.yml
  format: yaml
  label: Marketstack Dividends API
  slug: marketstack-dividends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketstack/refs/heads/main/openapi/marketstack-dividends-api-openapi.yml
- filename: marketstack-edgar-api-openapi.yml
  format: yaml
  label: Marketstack EDGAR API
  slug: marketstack-edgar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketstack/refs/heads/main/openapi/marketstack-edgar-api-openapi.yml
- filename: marketstack-end-of-day-api-openapi.yml
  format: yaml
  label: Marketstack End Of Day API
  slug: marketstack-end-of-day-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketstack/refs/heads/main/openapi/marketstack-end-of-day-api-openapi.yml
- filename: marketstack-etfs-api-openapi.yml
  format: yaml
  label: Marketstack ET Fs API
  slug: marketstack-etfs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketstack/refs/heads/main/openapi/marketstack-etfs-api-openapi.yml
- filename: marketstack-exchanges-api-openapi.yml
  format: yaml
  label: Marketstack Exchanges API
  slug: marketstack-exchanges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketstack/refs/heads/main/openapi/marketstack-exchanges-api-openapi.yml
- filename: marketstack-indexes-api-openapi.yml
  format: yaml
  label: Marketstack Indexes API
  slug: marketstack-indexes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketstack/refs/heads/main/openapi/marketstack-indexes-api-openapi.yml
- filename: marketstack-intraday-api-openapi.yml
  format: yaml
  label: Marketstack Intraday API
  slug: marketstack-intraday-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketstack/refs/heads/main/openapi/marketstack-intraday-api-openapi.yml
- filename: marketstack-splits-api-openapi.yml
  format: yaml
  label: Marketstack Splits API
  slug: marketstack-splits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketstack/refs/heads/main/openapi/marketstack-splits-api-openapi.yml
- filename: marketstack-stock-prices-api-openapi.yml
  format: yaml
  label: Marketstack Stock Prices API
  slug: marketstack-stock-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketstack/refs/heads/main/openapi/marketstack-stock-prices-api-openapi.yml
- filename: marketstack-tickers-api-openapi.yml
  format: yaml
  label: Marketstack Tickers API
  slug: marketstack-tickers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketstack/refs/heads/main/openapi/marketstack-tickers-api-openapi.yml
- filename: marketstack-timezones-api-openapi.yml
  format: yaml
  label: Marketstack Timezones API
  slug: marketstack-timezones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketstack/refs/heads/main/openapi/marketstack-timezones-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Marketstack Authentication
name_suffix: Authentication
oauth_flows: []
overview: Marketstack secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Marketstack
provider_slug: marketstack
scheme_count: 1
schemes:
- description: 'Your Marketstack API access key. Every API request is authenticated by passing the account''s API access key to the access_key query parameter (format: access_key=YOUR_ACCESS_KEY). Keys are issued on signup and can be reset at any time from the account dashboard; the docs warn never to expose the key publicly. Unauthenticated requests receive HTTP 401 with error codes missing_access_key or invalid_access_key (verified by live probe 2026-07-22).'
  in: query
  name: ApiKeyQuery
  parameter: access_key
  sources:
  - openapi/marketstack-v2-openapi.json
  - https://docs.apilayer.com/marketstack/docs/api-documentation
  type: apiKey
slug: marketstack-authentication
source_filename: marketstack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: openapi/marketstack-v2-openapi.json\ndocs: https://docs.apilayer.com/marketstack/docs/api-documentation\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: access_key\n  description: >-\n    Your Marketstack API access key. Every API request is authenticated by\n    passing the account's API access key to the access_key query parameter\n    (format: access_key=YOUR_ACCESS_KEY). Keys are issued on signup and can be\n    reset at any time from the account dashboard; the docs warn never to expose\n    the key publicly. Unauthenticated requests receive HTTP 401 with error\n    codes missing_access_key or invalid_access_key (verified by live probe\n    2026-07-22).\n  sources:\n  - openapi/marketstack-v2-openapi.json\n  - https://docs.apilayer.com/marketstack/docs/api-documentation\nnotes: >-\n  No OAuth, no scopes - a single account-level API key governs\
  \ access; plan\n  tier (Free through Enterprise) determines which endpoints and features the\n  key can reach (higher-tier endpoints return 403 function_access_restricted).\n  HTTPS is supported on all current plans per the 2026 pricing page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marketstack/refs/heads/main/authentication/marketstack-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Finance
- Stock Market
- Market Data
- End-of-Day Data
- Intraday Data
- Commodities
- Bonds
- ETFs
- SEC EDGAR
- Dividends
---
