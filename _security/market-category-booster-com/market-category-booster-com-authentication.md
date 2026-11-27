---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: market-category-booster-com-categorizations-api-openapi.yml
  format: yaml
  label: Market Category Booster Categorizations API
  slug: market-category-booster-com-categorizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/market-category-booster-com/openapi/market-category-booster-com-categorizations-api-openapi.yml
- filename: market-category-booster-com-service-api-openapi.yml
  format: yaml
  label: Market Category Booster Service API
  slug: market-category-booster-com-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/market-category-booster-com/openapi/market-category-booster-com-service-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Market Category Booster Authentication
name_suffix: Authentication
oauth_flows: []
overview: Market Category Booster secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Market Category Booster
provider_slug: market-category-booster-com
scheme_count: 1
schemes:
- in: header
  name: APIKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/market-category-booster-com-openapi.json
  type: apiKey
slug: market-category-booster-com-authentication
source_filename: market-category-booster-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/market-category-booster-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/market-category-booster-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/market-category-booster-com/authentication/market-category-booster-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Marketplace
- Taxonomy
- MCP
- Product Categorization
---
