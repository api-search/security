---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Kalshi Trade API (REST)
  slug: trade-api
  spec_type: OpenAPI
  url: https://docs.kalshi.com/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Kalshi Trade API (external-api host)
  slug: trade-api-external
  spec_type: OpenAPI
  url: https://docs.kalshi.com/openapi.yaml
- filename: asyncapi.yaml
  format: yaml
  label: Kalshi WebSocket Streaming API
  slug: websocket
  spec_type: AsyncAPI
  url: https://docs.kalshi.com/asyncapi.yaml
- filename: openapi.yaml
  format: yaml
  label: Kalshi OpenAPI Specification
  slug: openapi
  spec_type: OpenAPI
  url: https://docs.kalshi.com/openapi.yaml
- filename: asyncapi.yaml
  format: yaml
  label: Kalshi AsyncAPI Specification
  slug: asyncapi
  spec_type: AsyncAPI
  url: https://docs.kalshi.com/asyncapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Kalshi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kalshi secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kalshi
provider_slug: kalshi
scheme_count: 3
schemes:
- description: Your API key ID
  in: header
  name: kalshiAccessKey
  parameter: KALSHI-ACCESS-KEY
  sources:
  - openapi/kalshi-openapi.yml
  type: apiKey
- description: RSA-PSS signature of the request
  in: header
  name: kalshiAccessSignature
  parameter: KALSHI-ACCESS-SIGNATURE
  sources:
  - openapi/kalshi-openapi.yml
  type: apiKey
- description: Request timestamp in milliseconds
  in: header
  name: kalshiAccessTimestamp
  parameter: KALSHI-ACCESS-TIMESTAMP
  sources:
  - openapi/kalshi-openapi.yml
  type: apiKey
slug: kalshi-authentication
source_filename: kalshi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kalshi-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: kalshiAccessKey\n  type: apiKey\n  in: header\n  parameter: KALSHI-ACCESS-KEY\n  description: Your API key ID\n  sources:\n  - openapi/kalshi-openapi.yml\n- name: kalshiAccessSignature\n  type: apiKey\n  in: header\n  parameter: KALSHI-ACCESS-SIGNATURE\n  description: RSA-PSS signature of the request\n  sources:\n  - openapi/kalshi-openapi.yml\n- name: kalshiAccessTimestamp\n  type: apiKey\n  in: header\n  parameter: KALSHI-ACCESS-TIMESTAMP\n  description: Request timestamp in milliseconds\n  sources:\n  - openapi/kalshi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kalshi/refs/heads/main/authentication/kalshi-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Prediction Markets
- Event Contracts
- Exchange
- CFTC
- Trading
- Markets
---
