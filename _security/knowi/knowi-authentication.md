---
api_key_in:
- header
api_specs:
- filename: knowi-management-api-openapi.yml
  format: yaml
  label: Knowi Management API
  slug: knowi-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knowi/refs/heads/main/openapi/knowi-management-api-openapi.yml
- filename: knowi-push-data-api-openapi.yml
  format: yaml
  label: Knowi Push Data API
  slug: knowi-push-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knowi/refs/heads/main/openapi/knowi-push-data-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Knowi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Knowi secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Knowi
provider_slug: knowi
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/knowi-management-api-openapi.yml
  type: http
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/knowi-push-data-api-openapi.yml
  type: apiKey
slug: knowi-authentication
source_filename: knowi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/knowi-management-api-openapi.yml, openapi/knowi-push-data-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/knowi-management-api-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/knowi-push-data-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knowi/refs/heads/main/authentication/knowi-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- AI Analytics
- API Analytics
- Business Intelligence
- Data Visualization
- Embedded Analytics
- NoSQL Analytics
---
