---
api_key_in: []
api_specs:
- filename: rest
  format: yaml
  label: Google Looker Studio API
  slug: google-looker-studio-api
  spec_type: OpenAPI
  url: https://lookerstudio.googleapis.com/$discovery/rest
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Looker Studio Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Looker Studio secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Looker Studio
provider_slug: google-looker-studio
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  sources:
  - openapi/google-looker-studio-openapi.yml
  type: oauth2
slug: google-looker-studio-authentication
source_filename: google-looker-studio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-looker-studio-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 3\n  sources:\n  - openapi/google-looker-studio-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-looker-studio/refs/heads/main/authentication/google-looker-studio-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Visualization
- Google
- Looker
- Reporting
---
