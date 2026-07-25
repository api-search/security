---
api_key_in:
- header
api_specs:
- filename: asyncapi.yaml
  format: yaml
  label: Kalshi WebSocket Streaming API
  slug: websocket
  spec_type: AsyncAPI
  url: https://docs.kalshi.com/asyncapi.yaml
- filename: asyncapi.yaml
  format: yaml
  label: Kalshi AsyncAPI Specification
  slug: asyncapi
  spec_type: AsyncAPI
  url: https://docs.kalshi.com/asyncapi.yaml
- filename: kalshi-account-api-openapi.yml
  format: yaml
  label: Kalshi account API
  slug: kalshi-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kalshi/refs/heads/main/openapi/kalshi-account-api-openapi.yml
- filename: kalshi-api-keys-api-openapi.yml
  format: yaml
  label: Kalshi api-keys API
  slug: kalshi-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kalshi/refs/heads/main/openapi/kalshi-api-keys-api-openapi.yml
- filename: kalshi-communications-api-openapi.yml
  format: yaml
  label: Kalshi communications API
  slug: kalshi-communications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kalshi/refs/heads/main/openapi/kalshi-communications-api-openapi.yml
- filename: kalshi-events-api-openapi.yml
  format: yaml
  label: Kalshi events API
  slug: kalshi-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kalshi/refs/heads/main/openapi/kalshi-events-api-openapi.yml
- filename: kalshi-exchange-api-openapi.yml
  format: yaml
  label: Kalshi exchange API
  slug: kalshi-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kalshi/refs/heads/main/openapi/kalshi-exchange-api-openapi.yml
- filename: kalshi-fcm-api-openapi.yml
  format: yaml
  label: Kalshi fcm API
  slug: kalshi-fcm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kalshi/refs/heads/main/openapi/kalshi-fcm-api-openapi.yml
- filename: kalshi-historical-api-openapi.yml
  format: yaml
  label: Kalshi historical API
  slug: kalshi-historical-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kalshi/refs/heads/main/openapi/kalshi-historical-api-openapi.yml
- filename: kalshi-incentive-programs-api-openapi.yml
  format: yaml
  label: Kalshi incentive-programs API
  slug: kalshi-incentive-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kalshi/refs/heads/main/openapi/kalshi-incentive-programs-api-openapi.yml
- filename: kalshi-live-data-api-openapi.yml
  format: yaml
  label: Kalshi live-data API
  slug: kalshi-live-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kalshi/refs/heads/main/openapi/kalshi-live-data-api-openapi.yml
- filename: kalshi-market-api-openapi.yml
  format: yaml
  label: Kalshi market API
  slug: kalshi-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kalshi/refs/heads/main/openapi/kalshi-market-api-openapi.yml
- filename: kalshi-milestone-api-openapi.yml
  format: yaml
  label: Kalshi milestone API
  slug: kalshi-milestone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kalshi/refs/heads/main/openapi/kalshi-milestone-api-openapi.yml
- filename: kalshi-multivariate-api-openapi.yml
  format: yaml
  label: Kalshi multivariate API
  slug: kalshi-multivariate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kalshi/refs/heads/main/openapi/kalshi-multivariate-api-openapi.yml
- filename: kalshi-order-groups-api-openapi.yml
  format: yaml
  label: Kalshi order-groups API
  slug: kalshi-order-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kalshi/refs/heads/main/openapi/kalshi-order-groups-api-openapi.yml
- filename: kalshi-orders-api-openapi.yml
  format: yaml
  label: Kalshi orders API
  slug: kalshi-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kalshi/refs/heads/main/openapi/kalshi-orders-api-openapi.yml
- filename: kalshi-portfolio-api-openapi.yml
  format: yaml
  label: Kalshi portfolio API
  slug: kalshi-portfolio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kalshi/refs/heads/main/openapi/kalshi-portfolio-api-openapi.yml
- filename: kalshi-search-api-openapi.yml
  format: yaml
  label: Kalshi search API
  slug: kalshi-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kalshi/refs/heads/main/openapi/kalshi-search-api-openapi.yml
- filename: kalshi-structured-targets-api-openapi.yml
  format: yaml
  label: Kalshi structured-targets API
  slug: kalshi-structured-targets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kalshi/refs/heads/main/openapi/kalshi-structured-targets-api-openapi.yml
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
