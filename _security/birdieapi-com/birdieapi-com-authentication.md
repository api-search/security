---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: birdieapi-com-basic-lookup-api-openapi.yml
  format: yaml
  label: birdieapi-com Basic lookup API
  slug: birdieapi-com-basic-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/birdieapi-com/openapi/birdieapi-com-basic-lookup-api-openapi.yml
- filename: birdieapi-com-static-reference-api-openapi.yml
  format: yaml
  label: birdieapi-com Static reference API
  slug: birdieapi-com-static-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/birdieapi-com/openapi/birdieapi-com-static-reference-api-openapi.yml
- filename: birdieapi-com-stats-aggregation-api-openapi.yml
  format: yaml
  label: birdieapi-com Stats + aggregation API
  slug: birdieapi-com-stats-aggregation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/birdieapi-com/openapi/birdieapi-com-stats-aggregation-api-openapi.yml
- filename: birdieapi-com-time-series-api-openapi.yml
  format: yaml
  label: birdieapi-com Time Series API
  slug: birdieapi-com-time-series-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/birdieapi-com/openapi/birdieapi-com-time-series-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Birdieapi Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: birdieapi-com secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: birdieapi-com
provider_slug: birdieapi-com
scheme_count: 2
schemes:
- in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/birdieapi-com-openapi.json
  type: apiKey
- description: The same API key as a bearer token.
  name: bearer
  scheme: bearer
  sources:
  - openapi/birdieapi-com-openapi.json
  type: http
slug: birdieapi-com-authentication
source_filename: birdieapi-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/birdieapi-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/birdieapi-com-openapi.json\n- name: bearer\n  type: http\n  scheme: bearer\n  description: The same API key as a bearer token.\n  sources:\n  - openapi/birdieapi-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/birdieapi-com/authentication/birdieapi-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Bird Tracking
- Migration Analytics
- Open Data
- Conservation
---
