---
api_key_in:
- query
- header
api_specs:
- filename: twelvedata-asyncapi.yml
  format: yaml
  label: Twelve Data WebSocket Streaming API
  slug: twelvedata-websocket-streaming-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvedata/refs/heads/main/asyncapi/twelvedata-asyncapi.yml
- filename: twelvedata-core-data-api-openapi.yml
  format: yaml
  label: Twelve Data Core Data API
  slug: twelvedata-core-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvedata/refs/heads/main/openapi/twelvedata-core-data-api-openapi.yml
- filename: twelvedata-fundamentals-api-openapi.yml
  format: yaml
  label: Twelve Data Fundamentals API
  slug: twelvedata-fundamentals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvedata/refs/heads/main/openapi/twelvedata-fundamentals-api-openapi.yml
- filename: twelvedata-reference-data-api-openapi.yml
  format: yaml
  label: Twelve Data Reference Data API
  slug: twelvedata-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvedata/refs/heads/main/openapi/twelvedata-reference-data-api-openapi.yml
- filename: twelvedata-technical-indicators-api-openapi.yml
  format: yaml
  label: Twelve Data Technical Indicators API
  slug: twelvedata-technical-indicators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvedata/refs/heads/main/openapi/twelvedata-technical-indicators-api-openapi.yml
- filename: twelvedata-time-series-api-openapi.yml
  format: yaml
  label: Twelve Data Time Series API
  slug: twelvedata-time-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvedata/refs/heads/main/openapi/twelvedata-time-series-api-openapi.yml
- filename: twelvedata-advanced-api-openapi.yml
  format: yaml
  label: Twelve Data Advanced API
  slug: twelvedata-advanced-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvedata/refs/heads/main/openapi/twelvedata-advanced-api-openapi.yml
- filename: twelvedata-analysis-api-openapi.yml
  format: yaml
  label: Twelve Data Analysis API
  slug: twelvedata-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvedata/refs/heads/main/openapi/twelvedata-analysis-api-openapi.yml
- filename: twelvedata-currencies-api-openapi.yml
  format: yaml
  label: Twelve Data Currencies API
  slug: twelvedata-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvedata/refs/heads/main/openapi/twelvedata-currencies-api-openapi.yml
- filename: twelvedata-etfs-api-openapi.yml
  format: yaml
  label: Twelve Data Etfs API
  slug: twelvedata-etfs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvedata/refs/heads/main/openapi/twelvedata-etfs-api-openapi.yml
- filename: twelvedata-market-data-api-openapi.yml
  format: yaml
  label: Twelve Data Market Data API
  slug: twelvedata-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvedata/refs/heads/main/openapi/twelvedata-market-data-api-openapi.yml
- filename: twelvedata-money-market-funds-api-openapi.yml
  format: yaml
  label: Twelve Data Money Market Funds API
  slug: twelvedata-money-market-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvedata/refs/heads/main/openapi/twelvedata-money-market-funds-api-openapi.yml
- filename: twelvedata-mutual-funds-api-openapi.yml
  format: yaml
  label: Twelve Data Mutual Funds API
  slug: twelvedata-mutual-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvedata/refs/heads/main/openapi/twelvedata-mutual-funds-api-openapi.yml
- filename: twelvedata-regulatory-api-openapi.yml
  format: yaml
  label: Twelve Data Regulatory API
  slug: twelvedata-regulatory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvedata/refs/heads/main/openapi/twelvedata-regulatory-api-openapi.yml
- filename: twelvedata-technical-indicator-api-openapi.yml
  format: yaml
  label: Twelve Data Technical Indicator API
  slug: twelvedata-technical-indicator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twelvedata/refs/heads/main/openapi/twelvedata-technical-indicator-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
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
  notes: API key supplied as the apikey query parameter, e.g. ?apikey=YOUR_API_KEY. Also used to authenticate the WebSocket connection URL. Matches securityScheme queryParameter in the provider-published OpenAPI.
  sources:
  - openapi/twelvedata-openapi-original.json
  type: apiKey
- format: apikey <KEY>
  in: header
  keyName: Authorization
  name: apikey_header
  notes: 'Recommended method — API key supplied via the Authorization header as: Authorization: apikey YOUR_API_KEY. Matches securityScheme authorizationHeader in the provider-published OpenAPI.'
  sources:
  - openapi/twelvedata-openapi-original.json
  type: apiKey
slug: twelvedata-authentication
source_filename: twelvedata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: https://twelvedata.com/docs/llms/introduction.md (Authentication section)\ndocs: https://twelvedata.com/docs\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\n  - header\nschemes:\n- name: apikey_query\n  type: apiKey\n  in: query\n  keyName: apikey\n  sources:\n  - openapi/twelvedata-openapi-original.json\n  notes: API key supplied as the apikey query parameter, e.g. ?apikey=YOUR_API_KEY.\n    Also used to authenticate the WebSocket connection URL. Matches securityScheme\n    queryParameter in the provider-published OpenAPI.\n- name: apikey_header\n  type: apiKey\n  in: header\n  keyName: Authorization\n  format: 'apikey <KEY>'\n  sources:\n  - openapi/twelvedata-openapi-original.json\n  notes: 'Recommended method — API key supplied via the Authorization header as:\n    Authorization: apikey YOUR_API_KEY. Matches securityScheme authorizationHeader\n    in the provider-published OpenAPI.'\nkey_issuance:\n  signup:\
  \ https://twelvedata.com/register\n  dashboard: https://twelvedata.com/account/api-keys\n  demo_key: apikey=demo (published demo key for demo requests)\nrelated:\n  mcp_oauth: >-\n    The hosted MCP server (https://mcp.twelvedata.com/mcp) fronts the API-key\n    model with OAuth 2.0 authorization-code + PKCE (RFC 8414 metadata captured\n    in well-known/twelvedata-mcp-oauth-authorization-server.json, scope\n    \"twelvedata\"); login links the user's Twelve Data API key.\n"
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
