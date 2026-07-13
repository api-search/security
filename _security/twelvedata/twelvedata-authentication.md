---
api_key_in: []
api_specs:
- filename: twelvedata-openapi.yml
  format: yaml
  label: Twelve Data Time Series API
  slug: twelvedata-time-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvedata/refs/heads/main/openapi/twelvedata-openapi.yml
- filename: twelvedata-openapi.yml
  format: yaml
  label: Twelve Data Quotes and Price API
  slug: twelvedata-quotes-price-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvedata/refs/heads/main/openapi/twelvedata-openapi.yml
- filename: twelvedata-openapi.yml
  format: yaml
  label: Twelve Data Technical Indicators API
  slug: twelvedata-technical-indicators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvedata/refs/heads/main/openapi/twelvedata-openapi.yml
- filename: twelvedata-openapi.yml
  format: yaml
  label: Twelve Data Reference Data API
  slug: twelvedata-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvedata/refs/heads/main/openapi/twelvedata-openapi.yml
- filename: twelvedata-openapi.yml
  format: yaml
  label: Twelve Data Fundamentals API
  slug: twelvedata-fundamentals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvedata/refs/heads/main/openapi/twelvedata-openapi.yml
- filename: twelvedata-asyncapi.yml
  format: yaml
  label: Twelve Data WebSocket Streaming API
  slug: twelvedata-websocket-streaming-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvedata/refs/heads/main/asyncapi/twelvedata-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Twelvedata Authentication
name_suffix: Authentication
oauth_flows: []
overview: Twelve Data secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Twelve Data
provider_slug: twelvedata
scheme_count: 2
schemes:
- in: query
  keyName: apikey
  name: apikey_query
  notes: API key supplied as the apikey query parameter, e.g. ?apikey=YOUR_API_KEY. Also used to authenticate the WebSocket connection URL.
  sources:
  - openapi/twelvedata-openapi.yml
  type: apiKey
- format: apikey <KEY>
  in: header
  keyName: Authorization
  name: apikey_header
  notes: 'API key supplied via the Authorization header as: Authorization: apikey YOUR_API_KEY.'
  sources:
  - openapi/twelvedata-openapi.yml
  type: apiKey
slug: twelvedata-authentication
source_filename: twelvedata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/twelvedata-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: apikey_query\n  type: apiKey\n  in: query\n  keyName: apikey\n  sources:\n  - openapi/twelvedata-openapi.yml\n  notes: API key supplied as the apikey query parameter, e.g. ?apikey=YOUR_API_KEY. Also used to authenticate the WebSocket connection URL.\n- name: apikey_header\n  type: apiKey\n  in: header\n  keyName: Authorization\n  format: 'apikey <KEY>'\n  sources:\n  - openapi/twelvedata-openapi.yml\n  notes: 'API key supplied via the Authorization header as: Authorization: apikey YOUR_API_KEY.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/twelvedata/refs/heads/main/authentication/twelvedata-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Market Data
- Financial Data
- Stocks
- Forex
- Crypto
- Real-Time Data
- Technical Indicators
- Fundamentals
---
