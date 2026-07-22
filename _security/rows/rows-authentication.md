---
api_key_in: []
api_specs:
- filename: rows-openapi.yml
  format: yaml
  label: Rows API
  slug: rows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rows/refs/heads/main/openapi/rows-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Rows Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rows secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rows
provider_slug: rows
scheme_count: 1
schemes:
- description: 'Rows API key sent as an Authorization: Bearer <API_KEY> header. Generate a key in your Rows account settings.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/rows-openapi.yml
  type: http
slug: rows-authentication
source_filename: rows-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/rows-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'Rows API key sent as an Authorization: Bearer <API_KEY> header. Generate a key\n    in your Rows account settings.'\n  sources:\n  - openapi/rows-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rows/refs/heads/main/authentication/rows-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Productivity
- Spreadsheets
- Data
- No-Code
- Automation
- Artificial Intelligence
- Analytics
- Business Intelligence
---
