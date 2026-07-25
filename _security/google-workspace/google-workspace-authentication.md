---
api_key_in: []
api_specs:
- filename: google-workspace-groups-api-openapi.yml
  format: yaml
  label: Google Workspace Groups API
  slug: google-workspace-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-workspace/refs/heads/main/openapi/google-workspace-groups-api-openapi.yml
- filename: google-workspace-orgunits-api-openapi.yml
  format: yaml
  label: Google Workspace OrgUnits API
  slug: google-workspace-orgunits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-workspace/refs/heads/main/openapi/google-workspace-orgunits-api-openapi.yml
- filename: google-workspace-users-api-openapi.yml
  format: yaml
  label: Google Workspace Users API
  slug: google-workspace-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-workspace/refs/heads/main/openapi/google-workspace-users-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Workspace Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Workspace secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Workspace
provider_slug: google-workspace
scheme_count: 1
schemes:
- description: OAuth 2.0 authorization for Google Workspace Admin operations.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/admin-sdk-directory-api.yml
  type: oauth2
slug: google-workspace-authentication
source_filename: google-workspace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/admin-sdk-directory-api.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 6\n  description: OAuth 2.0 authorization for Google Workspace Admin operations.\n  sources:\n  - openapi/admin-sdk-directory-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-workspace/refs/heads/main/authentication/google-workspace-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Calendar
- Collaboration
- Email
- Productivity
- Storage
- Video Conferencing
---
