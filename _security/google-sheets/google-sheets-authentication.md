---
api_key_in:
- query
api_specs:
- filename: google-sheets-openapi.yml
  format: yaml
  label: Google Sheets API v4
  slug: google-sheets-api-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/openapi/google-sheets-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Sheets Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Sheets secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Sheets
provider_slug: google-sheets
scheme_count: 2
schemes:
- description: OAuth 2.0 authentication for accessing user spreadsheets.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/google-sheets-openapi.yml
  type: oauth2
- description: API key for accessing public spreadsheets without user authentication.
  in: query
  name: apiKey
  parameter: key
  sources:
  - openapi/google-sheets-openapi.yml
  type: apiKey
slug: google-sheets-authentication
source_filename: google-sheets-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-sheets-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 5\n  description: OAuth 2.0 authentication for accessing user spreadsheets.\n  sources:\n  - openapi/google-sheets-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  description: API key for accessing public spreadsheets without user authentication.\n  sources:\n  - openapi/google-sheets-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/authentication/google-sheets-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Google Workspace
- Productivity
- Spreadsheets
---
