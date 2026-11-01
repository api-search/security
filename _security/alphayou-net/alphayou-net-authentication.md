---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: alphayou-net-alphayou-api-openapi.yml
  format: yaml
  label: alphayou-net Alpha You API
  slug: alphayou-net-alphayou-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alphayou-net/openapi/alphayou-net-alphayou-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Alphayou Net Authentication
name_suffix: Authentication
oauth_flows: []
overview: alphayou-net secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: alphayou-net
provider_slug: alphayou-net
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/alphayou-net-openapi.json
  type: apiKey
- description: Your AlphaYou API key (ay_...).
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/alphayou-net-openapi.json
  type: http
slug: alphayou-net-authentication
source_filename: alphayou-net-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: derived\nsource: openapi/alphayou-net-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/alphayou-net-openapi.json\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Your AlphaYou API key (ay_...).\n  sources:\n  - openapi/alphayou-net-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/alphayou-net/authentication/alphayou-net-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Finance
- StockResearch
- TradingTools
- MarketAnalytics
- Alerts
---
