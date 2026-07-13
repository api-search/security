---
api_key_in:
- header
api_specs:
- filename: alpaca-trading-api-openapi.yml
  format: yaml
  label: Alpaca Trading API
  slug: trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-trading-api-openapi.yml
- filename: alpaca-data-api-openapi.yml
  format: yaml
  label: Alpaca Market Data API
  slug: market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-data-api-openapi.yml
- filename: alpaca-broker-api-openapi.yml
  format: yaml
  label: Alpaca Broker API
  slug: broker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-broker-api-openapi.yml
- filename: alpaca-oauth-api-openapi.yml
  format: yaml
  label: Alpaca OAuth API
  slug: oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/openapi/alpaca-oauth-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Alpaca Authentication
name_suffix: Authentication
oauth_flows: []
overview: Alpaca secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Alpaca
provider_slug: alpaca
scheme_count: 3
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/alpaca-broker-api-openapi.yml
  type: http
- in: header
  name: API_Key
  parameter: APCA-API-KEY-ID
  sources:
  - openapi/alpaca-data-api-openapi.yml
  - openapi/alpaca-oauth-api-openapi.yml
  - openapi/alpaca-trading-api-openapi.yml
  type: apiKey
- in: header
  name: API_Secret
  parameter: APCA-API-SECRET-KEY
  sources:
  - openapi/alpaca-data-api-openapi.yml
  - openapi/alpaca-oauth-api-openapi.yml
  - openapi/alpaca-trading-api-openapi.yml
  type: apiKey
slug: alpaca-authentication
source_filename: alpaca-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/alpaca-broker-api-openapi.yml, openapi/alpaca-data-api-openapi.yml, openapi/alpaca-oauth-api-openapi.yml,\n  openapi/alpaca-trading-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/alpaca-broker-api-openapi.yml\n- name: API_Key\n  type: apiKey\n  in: header\n  parameter: APCA-API-KEY-ID\n  sources:\n  - openapi/alpaca-data-api-openapi.yml\n  - openapi/alpaca-oauth-api-openapi.yml\n  - openapi/alpaca-trading-api-openapi.yml\n- name: API_Secret\n  type: apiKey\n  in: header\n  parameter: APCA-API-SECRET-KEY\n  sources:\n  - openapi/alpaca-data-api-openapi.yml\n  - openapi/alpaca-oauth-api-openapi.yml\n  - openapi/alpaca-trading-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alpaca/refs/heads/main/authentication/alpaca-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Fintech
- Trading
- Stocks
- Crypto
- Brokerage
- Market Data
- Options
---
