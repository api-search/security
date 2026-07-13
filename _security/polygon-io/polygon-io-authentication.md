---
api_key_in:
- query
api_specs:
- filename: polygon-io-asyncapi.yml
  format: yaml
  label: Polygon.io Stocks API
  slug: stocks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-io/refs/heads/main/asyncapi/polygon-io-asyncapi.yml
- filename: polygon-io-asyncapi.yml
  format: yaml
  label: Polygon.io Options API
  slug: options-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-io/refs/heads/main/asyncapi/polygon-io-asyncapi.yml
- filename: polygon-io-asyncapi.yml
  format: yaml
  label: Polygon.io Indices API
  slug: indices-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-io/refs/heads/main/asyncapi/polygon-io-asyncapi.yml
- filename: polygon-io-asyncapi.yml
  format: yaml
  label: Polygon.io Forex API
  slug: forex-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-io/refs/heads/main/asyncapi/polygon-io-asyncapi.yml
- filename: polygon-io-asyncapi.yml
  format: yaml
  label: Polygon.io Crypto API
  slug: crypto-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-io/refs/heads/main/asyncapi/polygon-io-asyncapi.yml
- filename: polygon-io-asyncapi.yml
  format: yaml
  label: Polygon.io Futures API
  slug: futures-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygon-io/refs/heads/main/asyncapi/polygon-io-asyncapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Polygon Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Polygon.io secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Polygon.io
provider_slug: polygon-io
scheme_count: 2
schemes:
- in: query
  name: apiKeyQuery
  parameter: apiKey
  sources:
  - openapi/polygon-io-openapi.yml
  type: apiKey
- bearerFormat: API Key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/polygon-io-openapi.yml
  type: http
slug: polygon-io-authentication
source_filename: polygon-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/polygon-io-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: apiKey\n  sources:\n  - openapi/polygon-io-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  sources:\n  - openapi/polygon-io-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polygon-io/refs/heads/main/authentication/polygon-io-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
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
---
