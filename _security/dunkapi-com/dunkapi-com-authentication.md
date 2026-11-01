---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dunkapi-com-basic-lookup-api-openapi.yml
  format: yaml
  label: dunkapi-com Basic lookup API
  slug: dunkapi-com-basic-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dunkapi-com/openapi/dunkapi-com-basic-lookup-api-openapi.yml
- filename: dunkapi-com-multi-table-api-openapi.yml
  format: yaml
  label: dunkapi-com Multi Table API
  slug: dunkapi-com-multi-table-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dunkapi-com/openapi/dunkapi-com-multi-table-api-openapi.yml
- filename: dunkapi-com-static-reference-api-openapi.yml
  format: yaml
  label: dunkapi-com Static reference API
  slug: dunkapi-com-static-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dunkapi-com/openapi/dunkapi-com-static-reference-api-openapi.yml
- filename: dunkapi-com-stats-aggregation-api-openapi.yml
  format: yaml
  label: dunkapi-com Stats + aggregation API
  slug: dunkapi-com-stats-aggregation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dunkapi-com/openapi/dunkapi-com-stats-aggregation-api-openapi.yml
- filename: dunkapi-com-time-series-api-openapi.yml
  format: yaml
  label: dunkapi-com Time Series API
  slug: dunkapi-com-time-series-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dunkapi-com/openapi/dunkapi-com-time-series-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Dunkapi Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: dunkapi-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: dunkapi-com
provider_slug: dunkapi-com
scheme_count: 2
schemes:
- description: API key passed in header
  in: header
  name: x-api-key
  type: apiKey
- bearerFormat: JWT
  description: Bearer token alternative
  scheme: bearer
  type: http
slug: dunkapi-com-authentication
source_filename: dunkapi-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://dunkapi.com/docs\nname: DunkAPI authentication\nschemes:\n  - type: apiKey\n    name: x-api-key\n    in: header\n    description: API key passed in header\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: Bearer token alternative\n"
source_yaml_url: https://artifacts.apis.io/dunkapi-com/authentication/dunkapi-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Sports
- Basketball
- NBA
- Data
---
