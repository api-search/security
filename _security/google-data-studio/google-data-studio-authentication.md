---
api_key_in: []
api_specs:
- filename: google-data-studio-api-openapi.yml
  format: yaml
  label: Google Data Studio API
  slug: google-data-studio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-data-studio/refs/heads/main/openapi/google-data-studio-api-openapi.yml
- filename: google-data-studio-linking-api-openapi.yml
  format: yaml
  label: Looker Studio Linking API
  slug: looker-studio-linking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-data-studio/refs/heads/main/openapi/google-data-studio-linking-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Data Studio Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Data Studio secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Data Studio
provider_slug: google-data-studio
scheme_count: 1
schemes:
- description: OAuth 2.0 authentication. Requires domain-wide delegation configured by a Google Workspace administrator.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/google-data-studio-api-openapi.yml
  type: oauth2
slug: google-data-studio-authentication
source_filename: google-data-studio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-data-studio-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 3\n  description: OAuth 2.0 authentication. Requires domain-wide delegation configured by a Google\n    Workspace administrator.\n  sources:\n  - openapi/google-data-studio-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-data-studio/refs/heads/main/authentication/google-data-studio-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data
- Reporting
- Visualization
---
