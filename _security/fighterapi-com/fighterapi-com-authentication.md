---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fighterapi-com-basic-lookup-api-openapi.yml
  format: yaml
  label: fighterapi-com Basic lookup API
  slug: fighterapi-com-basic-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fighterapi-com/openapi/fighterapi-com-basic-lookup-api-openapi.yml
- filename: fighterapi-com-static-reference-api-openapi.yml
  format: yaml
  label: fighterapi-com Static reference API
  slug: fighterapi-com-static-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fighterapi-com/openapi/fighterapi-com-static-reference-api-openapi.yml
- filename: fighterapi-com-stats-aggregation-api-openapi.yml
  format: yaml
  label: fighterapi-com Stats + aggregation API
  slug: fighterapi-com-stats-aggregation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fighterapi-com/openapi/fighterapi-com-stats-aggregation-api-openapi.yml
- filename: fighterapi-com-time-series-api-openapi.yml
  format: yaml
  label: fighterapi-com Time Series API
  slug: fighterapi-com-time-series-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fighterapi-com/openapi/fighterapi-com-time-series-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Fighterapi Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: fighterapi-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: fighterapi-com
provider_slug: fighterapi-com
scheme_count: 2
schemes:
- description: API key header
  in: header
  name: x-api-key
  type: apiKey
- description: API key as bearer token
  scheme: bearer
  type: http
slug: fighterapi-com-authentication
source_filename: fighterapi-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/_original/openapi.json\nschemes:\n  - type: apiKey\n    in: header\n    name: x-api-key\n    description: API key header\n  - type: http\n    scheme: bearer\n    description: API key as bearer token\n"
source_yaml_url: https://artifacts.apis.io/fighterapi-com/authentication/fighterapi-com-authentication.yml
summary_line: 2 schemes
tags:
- Sports
- MMA
- Data
- API
- Odds
---
