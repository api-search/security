---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: buildix-trade-deep-view-api-openapi.yml
  format: yaml
  label: Buildix Deep View API
  slug: buildix-trade-deep-view-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildix-trade/openapi/buildix-trade-deep-view-api-openapi.yml
- filename: buildix-trade-funding-arb-api-openapi.yml
  format: yaml
  label: Buildix Funding Arb API
  slug: buildix-trade-funding-arb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildix-trade/openapi/buildix-trade-funding-arb-api-openapi.yml
- filename: buildix-trade-pair-api-openapi.yml
  format: yaml
  label: Buildix Pair API
  slug: buildix-trade-pair-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildix-trade/openapi/buildix-trade-pair-api-openapi.yml
- filename: buildix-trade-screener-api-openapi.yml
  format: yaml
  label: Buildix Screener API
  slug: buildix-trade-screener-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildix-trade/openapi/buildix-trade-screener-api-openapi.yml
- filename: buildix-trade-signals-api-openapi.yml
  format: yaml
  label: Buildix Signals API
  slug: buildix-trade-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildix-trade/openapi/buildix-trade-signals-api-openapi.yml
- filename: buildix-trade-smart-money-api-openapi.yml
  format: yaml
  label: Buildix Smart Money API
  slug: buildix-trade-smart-money-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildix-trade/openapi/buildix-trade-smart-money-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Buildix Trade Authentication
name_suffix: Authentication
oauth_flows: []
overview: Buildix secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Buildix
provider_slug: buildix-trade
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/buildix-trade-openapi.json
  type: apiKey
slug: buildix-trade-authentication
source_filename: buildix-trade-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/buildix-trade-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/buildix-trade-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/buildix-trade/authentication/buildix-trade-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Cryptocurrency
- Analytics
- Orderflow
- Artificial Intelligence
---
