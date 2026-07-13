---
api_key_in: []
api_specs:
- filename: zoom-api.yaml
  format: yaml
  label: Zoom API
  slug: zoom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/zoom/api/master/openapi/zoom-api.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Visioconference Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Visioconference secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Visioconference
provider_slug: visioconference
scheme_count: 1
schemes:
- description: OAuth 2.0 (server-to-server or user OAuth); access tokens valid for one hour
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://zoom.us/oauth/token
  - authorizationUrl: https://zoom.us/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://zoom.us/oauth/token
  name: oauth2
  sources:
  - openapi/visioconference-openapi.yml
  type: oauth2
slug: visioconference-authentication
source_filename: visioconference-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/visioconference-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://zoom.us/oauth/token\n    scopes: 0\n  - flow: authorizationCode\n    authorizationUrl: https://zoom.us/oauth/authorize\n    tokenUrl: https://zoom.us/oauth/token\n    scopes: 0\n  description: OAuth 2.0 (server-to-server or user OAuth); access tokens valid for one hour\n  sources:\n  - openapi/visioconference-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/visioconference/refs/heads/main/authentication/visioconference-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Audio
- Chat
- Collaboration
- Communication
- Conferencing
- Live Streaming
- Real-Time
- Remote Work
- Screen Sharing
- Video
- WebRTC
---
