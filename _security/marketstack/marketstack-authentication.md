---
api_key_in:
- query
api_specs:
- filename: marketstack-v2-openapi.json
  format: json
  label: Marketstack API v2
  slug: marketstack-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketstack/refs/heads/main/openapi/marketstack-v2-openapi.json
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
