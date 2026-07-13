---
api_key_in:
- query
api_specs:
- filename: polygon-stocks-openapi.yml
  format: yaml
  label: Polygon Stocks API
  slug: stocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-stocks-openapi.yml
- filename: polygon-options-openapi.yml
  format: yaml
  label: Polygon Options API
  slug: options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-options-openapi.yml
- filename: polygon-indices-openapi.yml
  format: yaml
  label: Polygon Indices API
  slug: indices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-indices-openapi.yml
- filename: polygon-forex-openapi.yml
  format: yaml
  label: Polygon Forex API
  slug: forex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-forex-openapi.yml
- filename: polygon-crypto-openapi.yml
  format: yaml
  label: Polygon Crypto API
  slug: crypto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-crypto-openapi.yml
- filename: polygon-reference-openapi.yml
  format: yaml
  label: Polygon Reference API
  slug: reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/openapi/polygon-reference-openapi.yml
- filename: polygon-websocket-asyncapi.yml
  format: yaml
  label: Polygon WebSocket API
  slug: websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon/refs/heads/main/asyncapi/polygon-websocket-asyncapi.yml
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
  - openapi/polygon-crypto-openapi.yml
  - openapi/polygon-forex-openapi.yml
  - openapi/polygon-indices-openapi.yml
  - openapi/polygon-options-openapi.yml
  - openapi/polygon-reference-openapi.yml
  - openapi/polygon-stocks-openapi.yml
  type: apiKey
- bearerFormat: API Key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/polygon-crypto-openapi.yml
  - openapi/polygon-forex-openapi.yml
  - openapi/polygon-indices-openapi.yml
  - openapi/polygon-options-openapi.yml
  - openapi/polygon-reference-openapi.yml
  - openapi/polygon-stocks-openapi.yml
  type: http
slug: polygon-authentication
source_filename: polygon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/polygon-crypto-openapi.yml, openapi/polygon-forex-openapi.yml, openapi/polygon-indices-openapi.yml,\n  openapi/polygon-options-openapi.yml, openapi/polygon-reference-openapi.yml, openapi/polygon-stocks-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: apiKey\n  sources:\n  - openapi/polygon-crypto-openapi.yml\n  - openapi/polygon-forex-openapi.yml\n  - openapi/polygon-indices-openapi.yml\n  - openapi/polygon-options-openapi.yml\n  - openapi/polygon-reference-openapi.yml\n  - openapi/polygon-stocks-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  sources:\n  - openapi/polygon-crypto-openapi.yml\n  - openapi/polygon-forex-openapi.yml\n  - openapi/polygon-indices-openapi.yml\n  - openapi/polygon-options-openapi.yml\n  - openapi/polygon-reference-openapi.yml\n  - openapi/polygon-stocks-openapi.yml\n"
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
