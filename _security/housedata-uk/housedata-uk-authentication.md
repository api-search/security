---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: housedata-uk-scoring-api-openapi.yml
  format: yaml
  label: HouseData.uk Scoring API
  slug: housedata-uk-scoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/housedata-uk/openapi/housedata-uk-scoring-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: HouseData.uk Authentication
name_suffix: Authentication
oauth_flows: []
overview: HouseData.uk secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: HouseData.uk
provider_slug: housedata-uk
scheme_count: 2
schemes:
- description: 'API key as a bearer token: `Authorization: Bearer hd_prism_…`'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/housedata-uk-openapi.json
  type: http
- in: header
  name: apiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/housedata-uk-openapi.json
  type: apiKey
slug: housedata-uk-authentication
source_filename: housedata-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/housedata-uk-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key as a bearer token: `Authorization: Bearer hd_prism_…`'\n  sources:\n  - openapi/housedata-uk-openapi.json\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/housedata-uk-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/housedata-uk/authentication/housedata-uk-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Property
- Data
- United Kingdom
- Free
---
