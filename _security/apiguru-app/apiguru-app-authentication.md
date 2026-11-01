---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: apiguru-app-amazon-data-api-openapi.yml
  format: yaml
  label: apiguru-app Amazon Data API
  slug: apiguru-app-amazon-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apiguru-app/openapi/apiguru-app-amazon-data-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Apiguru App Authentication
name_suffix: Authentication
oauth_flows: []
overview: apiguru-app secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: apiguru-app
provider_slug: apiguru-app
scheme_count: 2
schemes:
- in: header
  name: ApiKeyHeader
  parameter: X-API-KEY
  sources:
  - openapi/apiguru-app-openapi.json
  type: apiKey
- in: query
  name: ApiKeyQuery
  parameter: api_key
  sources:
  - openapi/apiguru-app-openapi.json
  type: apiKey
slug: apiguru-app-authentication
source_filename: apiguru-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/apiguru-app-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/apiguru-app-openapi.json\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/apiguru-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/apiguru-app/authentication/apiguru-app-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- API
- Data
- Amazon
- Real-time
- Integration
---
