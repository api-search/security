---
api_key_in:
- header
api_specs:
- filename: tableau-desktop-openapi.yml
  format: yaml
  label: Tableau REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tableau-desktop/refs/heads/main/openapi/tableau-desktop-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tableau Desktop Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tableau Desktop secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tableau Desktop
provider_slug: tableau-desktop
scheme_count: 1
schemes:
- description: Authentication token returned by the Sign In endpoint.
  in: header
  name: tableauAuth
  parameter: X-Tableau-Auth
  sources:
  - openapi/tableau-desktop-openapi.yml
  type: apiKey
slug: tableau-desktop-authentication
source_filename: tableau-desktop-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tableau-desktop-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: tableauAuth\n  type: apiKey\n  in: header\n  parameter: X-Tableau-Auth\n  description: Authentication token returned by the Sign In endpoint.\n  sources:\n  - openapi/tableau-desktop-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tableau-desktop/refs/heads/main/authentication/tableau-desktop-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Analytics
- Business Intelligence
- Data Visualization
- Desktop Application
---
