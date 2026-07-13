---
api_key_in: []
api_specs:
- filename: rest
  format: yaml
  label: Google Meet REST API v2
  slug: rest-api-v2
  spec_type: OpenAPI
  url: https://meet.googleapis.com/$discovery/rest?version=v2
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Meet Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Meet secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Meet
provider_slug: meet
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/meet-openapi.yml
  type: oauth2
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/meet-openapi.yml
  type: http
slug: meet-authentication
source_filename: meet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/meet-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 3\n  sources:\n  - openapi/meet-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/meet-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meet/refs/heads/main/authentication/meet-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Video Conferencing
- Meetings
- Communication
- Collaboration
- Google Workspace
- Recordings
- Transcripts
---
