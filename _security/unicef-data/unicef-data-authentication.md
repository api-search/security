---
api_key_in:
- header
api_specs:
- filename: swagger.json
  format: json
  label: UNICEF Reference Data Manager API
  slug: unicef-reference-data-manager-api
  spec_type: OpenAPI
  url: https://rdmapi.unicef.org/swagger/v1/swagger.json
- filename: openapi.yaml
  format: yaml
  label: UNICEF GeoSight API
  slug: unicef-geosight-api
  spec_type: OpenAPI
  url: https://geosight.unicef.org/en-us/api/v1/docs/?format=openapi
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Unicef Data Authentication
name_suffix: Authentication
oauth_flows: []
overview: UNICEF Data secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: UNICEF Data
provider_slug: unicef-data
scheme_count: 1
schemes:
- in: header
  name: ApiKey Auth
  parameter: Authorization
  sources:
  - openapi/unicef-geosight-openapi.json
  type: apiKey
slug: unicef-data-authentication
source_filename: unicef-data-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/unicef-geosight-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey Auth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/unicef-geosight-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unicef-data/refs/heads/main/authentication/unicef-data-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Children
- Child Welfare
- Global Health
- Statistics
- SDG
- MICS
- Education
- Nutrition
- SDMX
- Open Data
- United Nations
- UNICEF
---
