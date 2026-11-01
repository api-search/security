---
anonymous_access: false
api_key_in: []
api_specs:
- filename: tickfeed-pro-account-api-openapi.yml
  format: yaml
  label: tickfeed-pro Account API
  slug: tickfeed-pro-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickfeed-pro/openapi/tickfeed-pro-account-api-openapi.yml
- filename: tickfeed-pro-market-data-api-openapi.yml
  format: yaml
  label: tickfeed-pro market data API
  slug: tickfeed-pro-market-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickfeed-pro/openapi/tickfeed-pro-market-data-api-openapi.yml
- filename: tickfeed-pro-system-api-openapi.yml
  format: yaml
  label: tickfeed-pro System API
  slug: tickfeed-pro-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickfeed-pro/openapi/tickfeed-pro-system-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Tickfeed Pro Authentication
name_suffix: Authentication
oauth_flows: []
overview: tickfeed-pro declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: tickfeed-pro
provider_slug: tickfeed-pro
scheme_count: 1
schemes:
- description: API key provided in the X-API-Key header.
  in: header
  name: X-API-Key
  type: apiKey
slug: tickfeed-pro-authentication
source_filename: tickfeed-pro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: https://tickfeed.pro/openapi.json\nschemes:\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    description: API key provided in the X-API-Key header.\n"
source_yaml_url: https://artifacts.apis.io/tickfeed-pro/authentication/tickfeed-pro-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Finance
- MarketData
- API
- Forex
- Gold
- MCP
---
