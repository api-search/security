---
api_key_in: []
api_specs:
- filename: google-sheets-openapi.yml
  format: yaml
  label: Google Sheets API
  slug: google-sheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spreadsheets/refs/heads/main/openapi/google-sheets-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Spreadsheets Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Spreadsheets secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Spreadsheets
provider_slug: spreadsheets
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  sources:
  - openapi/google-sheets-openapi.yml
  type: oauth2
slug: spreadsheets-authentication
source_filename: spreadsheets-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-sheets-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 2\n  sources:\n  - openapi/google-sheets-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spreadsheets/refs/heads/main/authentication/spreadsheets-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Spreadsheets
- Data
- Google Sheets
- Excel
- Productivity
- Automation
---
