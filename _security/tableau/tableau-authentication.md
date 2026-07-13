---
api_key_in:
- header
api_specs:
- filename: tableau-rest-api-openapi.yml
  format: yaml
  label: Tableau REST API
  slug: tableau-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/openapi/tableau-rest-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tableau Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tableau secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tableau
provider_slug: tableau
scheme_count: 1
schemes:
- description: The authentication token obtained from the Sign In method. Include this token in the X-Tableau-Auth header of all subsequent requests.
  in: header
  name: TableauAuth
  parameter: X-Tableau-Auth
  sources:
  - openapi/tableau-rest-api-openapi.yml
  type: apiKey
slug: tableau-authentication
source_filename: tableau-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tableau-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: TableauAuth\n  type: apiKey\n  in: header\n  parameter: X-Tableau-Auth\n  description: The authentication token obtained from the Sign In method. Include this token\n    in the X-Tableau-Auth header of all subsequent requests.\n  sources:\n  - openapi/tableau-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/authentication/tableau-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Visualization
---
