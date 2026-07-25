---
api_key_in:
- query
api_specs:
- filename: polygon-websocket-asyncapi.yml
  format: yaml
  label: Polygon WebSocket API
  slug: websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/asyncapi/polygon-websocket-asyncapi.yml
- filename: polygon-aggregates-api-openapi.yml
  format: yaml
  label: Polygon Aggregates API
  slug: polygon-aggregates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-aggregates-api-openapi.yml
- filename: polygon-books-api-openapi.yml
  format: yaml
  label: Polygon Books API
  slug: polygon-books-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-books-api-openapi.yml
- filename: polygon-contracts-api-openapi.yml
  format: yaml
  label: Polygon Contracts API
  slug: polygon-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-contracts-api-openapi.yml
- filename: polygon-conversion-api-openapi.yml
  format: yaml
  label: Polygon Conversion API
  slug: polygon-conversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-conversion-api-openapi.yml
- filename: polygon-corporateactions-api-openapi.yml
  format: yaml
  label: Polygon CorporateActions API
  slug: polygon-corporateactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-corporateactions-api-openapi.yml
- filename: polygon-dailybars-api-openapi.yml
  format: yaml
  label: Polygon DailyBars API
  slug: polygon-dailybars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-dailybars-api-openapi.yml
- filename: polygon-markets-api-openapi.yml
  format: yaml
  label: Polygon Markets API
  slug: polygon-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-markets-api-openapi.yml
- filename: polygon-news-api-openapi.yml
  format: yaml
  label: Polygon News API
  slug: polygon-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-news-api-openapi.yml
- filename: polygon-quotes-api-openapi.yml
  format: yaml
  label: Polygon Quotes API
  slug: polygon-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-quotes-api-openapi.yml
- filename: polygon-snapshots-api-openapi.yml
  format: yaml
  label: Polygon Snapshots API
  slug: polygon-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-snapshots-api-openapi.yml
- filename: polygon-tickers-api-openapi.yml
  format: yaml
  label: Polygon Tickers API
  slug: polygon-tickers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-tickers-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Polygon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Polygon secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Polygon
provider_slug: polygon
scheme_count: 2
schemes:
- in: query
  name: apiKeyQuery
  parameter: apiKey
  sources:
  - openapi/polygon-aggregates-api-openapi.yml
  - openapi/polygon-books-api-openapi.yml
  - openapi/polygon-contracts-api-openapi.yml
  - openapi/polygon-conversion-api-openapi.yml
  - openapi/polygon-corporateactions-api-openapi.yml
  - openapi/polygon-dailybars-api-openapi.yml
  - openapi/polygon-markets-api-openapi.yml
  - openapi/polygon-news-api-openapi.yml
  - openapi/polygon-openapi-original.json
  - openapi/polygon-quotes-api-openapi.yml
  - openapi/polygon-snapshots-api-openapi.yml
  - openapi/polygon-tickers-api-openapi.yml
  type: apiKey
- bearerFormat: API Key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/polygon-aggregates-api-openapi.yml
  - openapi/polygon-books-api-openapi.yml
  - openapi/polygon-contracts-api-openapi.yml
  - openapi/polygon-conversion-api-openapi.yml
  - openapi/polygon-corporateactions-api-openapi.yml
  - openapi/polygon-dailybars-api-openapi.yml
  - openapi/polygon-markets-api-openapi.yml
  - openapi/polygon-news-api-openapi.yml
  - openapi/polygon-quotes-api-openapi.yml
  - openapi/polygon-snapshots-api-openapi.yml
  - openapi/polygon-tickers-api-openapi.yml
  type: http
slug: polygon-authentication
source_filename: polygon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: derived\nsource: openapi/polygon-aggregates-api-openapi.yml, openapi/polygon-books-api-openapi.yml, openapi/polygon-contracts-api-openapi.yml,\n  openapi/polygon-conversion-api-openapi.yml, openapi/polygon-corporateactions-api-openapi.yml,\n  openapi/polygon-dailybars-api-openapi.yml, openapi/polygon-markets-api-openapi.yml, openapi/polygon-news-api-openapi.yml,\n  openapi/polygon-openapi-original.json, openapi/polygon-quotes-api-openapi.yml, openapi/polygon-snapshots-api-openapi.yml,\n  openapi/polygon-tickers-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: apiKey\n  sources:\n  - openapi/polygon-aggregates-api-openapi.yml\n  - openapi/polygon-books-api-openapi.yml\n  - openapi/polygon-contracts-api-openapi.yml\n  - openapi/polygon-conversion-api-openapi.yml\n  - openapi/polygon-corporateactions-api-openapi.yml\n  - openapi/polygon-dailybars-api-openapi.yml\n\
  \  - openapi/polygon-markets-api-openapi.yml\n  - openapi/polygon-news-api-openapi.yml\n  - openapi/polygon-openapi-original.json\n  - openapi/polygon-quotes-api-openapi.yml\n  - openapi/polygon-snapshots-api-openapi.yml\n  - openapi/polygon-tickers-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  sources:\n  - openapi/polygon-aggregates-api-openapi.yml\n  - openapi/polygon-books-api-openapi.yml\n  - openapi/polygon-contracts-api-openapi.yml\n  - openapi/polygon-conversion-api-openapi.yml\n  - openapi/polygon-corporateactions-api-openapi.yml\n  - openapi/polygon-dailybars-api-openapi.yml\n  - openapi/polygon-markets-api-openapi.yml\n  - openapi/polygon-news-api-openapi.yml\n  - openapi/polygon-quotes-api-openapi.yml\n  - openapi/polygon-snapshots-api-openapi.yml\n  - openapi/polygon-tickers-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/authentication/polygon-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Finance
- Fintech
- Market Data
- Stocks
- Options
- Forex
- Crypto
- Indices
- Futures
- WebSockets
- Real-time
- Historical
- Public APIs
---
