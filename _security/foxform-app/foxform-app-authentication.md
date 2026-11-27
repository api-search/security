---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: foxform-app-analytics-api-openapi.yml
  format: yaml
  label: FoxForm Analytics API
  slug: foxform-app-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foxform-app/openapi/foxform-app-analytics-api-openapi.yml
- filename: foxform-app-forms-api-openapi.yml
  format: yaml
  label: FoxForm Forms API
  slug: foxform-app-forms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foxform-app/openapi/foxform-app-forms-api-openapi.yml
- filename: foxform-app-integrations-api-openapi.yml
  format: yaml
  label: FoxForm Integrations API
  slug: foxform-app-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foxform-app/openapi/foxform-app-integrations-api-openapi.yml
- filename: foxform-app-responses-api-openapi.yml
  format: yaml
  label: FoxForm Responses API
  slug: foxform-app-responses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foxform-app/openapi/foxform-app-responses-api-openapi.yml
- filename: foxform-app-users-api-openapi.yml
  format: yaml
  label: FoxForm Users API
  slug: foxform-app-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foxform-app/openapi/foxform-app-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: FoxForm Authentication
name_suffix: Authentication
oauth_flows: []
overview: FoxForm secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FoxForm
provider_slug: foxform-app
scheme_count: 1
schemes:
- description: 'FoxForm API key (ff_live_…), generated in the dashboard under "MCP & API". Also accepted as ''Authorization: Bearer ff_live_…'' or a ''?key='' query param. Keys are scoped read or read+write.'
  in: header
  name: ApiKey
  parameter: x-api-key
  sources:
  - openapi/foxform-app-openapi.json
  type: apiKey
slug: foxform-app-authentication
source_filename: foxform-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/foxform-app-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: 'FoxForm API key (ff_live_…), generated in the dashboard under \"MCP & API\". Also\n    accepted as ''Authorization: Bearer ff_live_…'' or a ''?key='' query param. Keys are scoped\n    read or read+write.'\n  sources:\n  - openapi/foxform-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/foxform-app/authentication/foxform-app-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Form Builder
- Surveys
- Quiz
- Artificial Intelligence
---
