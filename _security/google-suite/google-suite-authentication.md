---
api_key_in: []
api_specs:
- filename: google-suite-gmail-api-openapi.yml
  format: yaml
  label: Google Workspace (G Suite) Gmail API
  slug: google-suite-gmail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-suite/refs/heads/main/openapi/google-suite-gmail-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Suite Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Workspace (G Suite) secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Workspace (G Suite)
provider_slug: google-suite
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  sources:
  - openapi/google-suite-openapi.yml
  type: oauth2
slug: google-suite-authentication
source_filename: google-suite-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-suite-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 5\n  sources:\n  - openapi/google-suite-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-suite/refs/heads/main/authentication/google-suite-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Cloud
- Collaboration
- Enterprise
- Google
- Productivity
- Workspace
---
