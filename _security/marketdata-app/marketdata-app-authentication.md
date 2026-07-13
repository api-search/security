---
api_key_in: []
api_specs:
- filename: marketdata-app-openapi.yml
  format: yaml
  label: Market Data Stocks API
  slug: marketdata-app-stocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketdata-app/refs/heads/main/openapi/marketdata-app-openapi.yml
- filename: marketdata-app-openapi.yml
  format: yaml
  label: Market Data Options API
  slug: marketdata-app-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketdata-app/refs/heads/main/openapi/marketdata-app-openapi.yml
- filename: marketdata-app-openapi.yml
  format: yaml
  label: Market Data Indices API
  slug: marketdata-app-indices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketdata-app/refs/heads/main/openapi/marketdata-app-openapi.yml
- filename: marketdata-app-openapi.yml
  format: yaml
  label: Market Data Markets API
  slug: marketdata-app-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketdata-app/refs/heads/main/openapi/marketdata-app-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Marketdata App Authentication
name_suffix: Authentication
oauth_flows: []
overview: Market Data secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Market Data
provider_slug: marketdata-app
scheme_count: 1
schemes:
- description: 'Bearer token generated in the Market Data dashboard. Passed as `Authorization: Bearer YOUR_API_TOKEN`. The token may also be supplied via a `token` query parameter for quick browser or spreadsheet use. A single IP address per account is enforced.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/marketdata-app-openapi.yml
  - https://www.marketdata.app/docs/api/authentication/
  type: http
slug: marketdata-app-authentication
source_filename: marketdata-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/marketdata-app-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Bearer token generated in the Market Data dashboard. Passed as\n    `Authorization: Bearer YOUR_API_TOKEN`. The token may also be supplied via a\n    `token` query parameter for quick browser or spreadsheet use. A single IP\n    address per account is enforced.\n  sources:\n  - openapi/marketdata-app-openapi.yml\n  - https://www.marketdata.app/docs/api/authentication/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marketdata-app/refs/heads/main/authentication/marketdata-app-authentication.yml
summary_line: http · 1 scheme
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
