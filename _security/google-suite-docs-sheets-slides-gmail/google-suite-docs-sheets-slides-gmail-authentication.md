---
api_key_in: []
api_specs:
- filename: rest
  format: yaml
  label: Google Docs API
  slug: google-docs-api
  spec_type: OpenAPI
  url: https://docs.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Google Sheets API
  slug: google-sheets-api
  spec_type: OpenAPI
  url: https://sheets.googleapis.com/$discovery/rest?version=v4
- filename: rest
  format: yaml
  label: Google Slides API
  slug: google-slides-api
  spec_type: OpenAPI
  url: https://slides.googleapis.com/$discovery/rest?version=v1
- filename: rest
  format: yaml
  label: Gmail API
  slug: gmail-api
  spec_type: OpenAPI
  url: https://gmail.googleapis.com/$discovery/rest?version=v1
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Suite Docs Sheets Slides Gmail Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Workspace Suite secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Workspace Suite
provider_slug: google-suite-docs-sheets-slides-gmail
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://oauth2.googleapis.com/token
  name: googleOAuth
  sources:
  - openapi/google-suite-docs-sheets-slides-gmail-openapi.yml
  type: oauth2
slug: google-suite-docs-sheets-slides-gmail-authentication
source_filename: google-suite-docs-sheets-slides-gmail-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-suite-docs-sheets-slides-gmail-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: googleOAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 6\n  sources:\n  - openapi/google-suite-docs-sheets-slides-gmail-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-suite-docs-sheets-slides-gmail/refs/heads/main/authentication/google-suite-docs-sheets-slides-gmail-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Cloud
- Collaboration
- Documents
- Google
- Productivity
- Workspace
---
