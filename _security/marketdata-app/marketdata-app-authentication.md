---
api_key_in:
- query
api_specs:
- filename: marketdata-app-indices-api-openapi.yml
  format: yaml
  label: Market Data Indices API
  slug: marketdata-app-indices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketdata-app/refs/heads/main/openapi/marketdata-app-indices-api-openapi.yml
- filename: marketdata-app-markets-api-openapi.yml
  format: yaml
  label: Market Data Markets API
  slug: marketdata-app-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketdata-app/refs/heads/main/openapi/marketdata-app-markets-api-openapi.yml
- filename: marketdata-app-options-api-openapi.yml
  format: yaml
  label: Market Data Options API
  slug: marketdata-app-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketdata-app/refs/heads/main/openapi/marketdata-app-options-api-openapi.yml
- filename: marketdata-app-stocks-api-openapi.yml
  format: yaml
  label: Market Data Stocks API
  slug: marketdata-app-stocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketdata-app/refs/heads/main/openapi/marketdata-app-stocks-api-openapi.yml
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Marketdata App Authentication
name_suffix: Authentication
oauth_flows: []
overview: Market Data secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Market Data
provider_slug: marketdata-app
scheme_count: 2
schemes:
- description: Bearer token generated in the Market Data customer dashboard (delivered by email) and passed in the Authorization header. The token is a programmatic representation of the account credentials and must be kept secret.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/marketdata-app-openapi-original.yml
  - https://www.marketdata.app/docs/api/authentication/
  type: http
- description: A read-only access token may be supplied as a token query parameter for quick browser or spreadsheet use. The provider discourages this - tokens in URLs are exposed in server logs and caches - and recommends header authentication.
  in: query
  name: tokenQueryParameter
  parameter: token
  sources:
  - https://www.marketdata.app/docs/api/universal-parameters/token/
  type: apiKey
slug: marketdata-app-authentication
source_filename: marketdata-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: https://www.marketdata.app/docs/api/authentication/\ndocs: https://www.marketdata.app/docs/api/authentication/\nsummary:\n  types:\n  - http\n  - apiKey\n  api_key_in:\n  - query\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Bearer token generated in the Market Data customer dashboard (delivered by\n    email) and passed in the Authorization header. The token is a programmatic\n    representation of the account credentials and must be kept secret.\n  sources:\n  - openapi/marketdata-app-openapi-original.yml\n  - https://www.marketdata.app/docs/api/authentication/\n- name: tokenQueryParameter\n  type: apiKey\n  in: query\n  parameter: token\n  description: >-\n    A read-only access token may be supplied as a token query parameter for\n    quick browser or spreadsheet use. The provider discourages this - tokens\n    in URLs are exposed in server logs and caches - and\
  \ recommends header\n    authentication.\n  sources:\n  - https://www.marketdata.app/docs/api/universal-parameters/token/\npolicies:\n  single_ip: >-\n    Each account may only connect from one IP address at a time; switching\n    back and forth between IPs within a 5-minute window triggers a temporary\n    block (HTTP 403).\n  demo_without_auth: >-\n    Stock endpoints with AAPL, options endpoints with any AAPL contract\n    (e.g. AAPL271217C00250000), and fund endpoints with VFINX work with no\n    token at all (historical data only).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marketdata-app/refs/heads/main/authentication/marketdata-app-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Market Data
- Financial Data
- Stocks
- Options
- Indices
- Real-Time Data
- Historical Data
- Quotes
---
