---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: acesapi-com-basic-lookup-api-openapi.yml
  format: yaml
  label: acesapi-com Basic lookup API
  slug: acesapi-com-basic-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acesapi-com/openapi/acesapi-com-basic-lookup-api-openapi.yml
- filename: acesapi-com-multi-table-api-openapi.yml
  format: yaml
  label: acesapi-com Multi Table API
  slug: acesapi-com-multi-table-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acesapi-com/openapi/acesapi-com-multi-table-api-openapi.yml
- filename: acesapi-com-static-reference-api-openapi.yml
  format: yaml
  label: acesapi-com Static reference API
  slug: acesapi-com-static-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acesapi-com/openapi/acesapi-com-static-reference-api-openapi.yml
- filename: acesapi-com-stats-aggregation-api-openapi.yml
  format: yaml
  label: acesapi-com Stats + aggregation API
  slug: acesapi-com-stats-aggregation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/acesapi-com/openapi/acesapi-com-stats-aggregation-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Acesapi Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: acesapi-com secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: acesapi-com
provider_slug: acesapi-com
scheme_count: 2
schemes:
- in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/acesapi-com-openapi.json
  type: apiKey
- description: The same API key as a bearer token.
  name: bearer
  scheme: bearer
  sources:
  - openapi/acesapi-com-openapi.json
  type: http
slug: acesapi-com-authentication
source_filename: acesapi-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/acesapi-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/acesapi-com-openapi.json\n- name: bearer\n  type: http\n  scheme: bearer\n  description: The same API key as a bearer token.\n  sources:\n  - openapi/acesapi-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/acesapi-com/authentication/acesapi-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Tennis
- Sports
- Data
- API
- MCP
- Rankings
---
