---
api_key_in:
- cookie
- header
api_specs:
- filename: openapi.json
  format: json
  label: Lightdash REST API
  slug: lightdash-rest-api
  spec_type: OpenAPI
  url: https://docs.lightdash.com/api-reference/openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Lightdash Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lightdash secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Lightdash
provider_slug: lightdash
scheme_count: 2
schemes:
- in: cookie
  name: session_cookie
  parameter: connect.sid
  sources:
  - openapi/lightdash-rest-api-openapi.yml
  type: apiKey
- description: Value should be 'ApiKey <your key>'
  in: header
  name: api_key
  parameter: Authorization
  sources:
  - openapi/lightdash-rest-api-openapi.yml
  type: apiKey
slug: lightdash-authentication
source_filename: lightdash-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lightdash-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: session_cookie\n  type: apiKey\n  in: cookie\n  parameter: connect.sid\n  sources:\n  - openapi/lightdash-rest-api-openapi.yml\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Value should be 'ApiKey <your key>'\n  sources:\n  - openapi/lightdash-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightdash/refs/heads/main/authentication/lightdash-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Business Intelligence
- Analytics
- dbt
- Semantic Layer
- Open Source
- Dashboards
- Data
---
