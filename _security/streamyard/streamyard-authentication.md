---
api_key_in: []
api_specs:
- filename: streamyard-openapi.yml
  format: yaml
  label: StreamYard API
  slug: streamyard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streamyard/refs/heads/main/openapi/streamyard-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Streamyard Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: StreamYard secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: StreamYard
provider_slug: streamyard
scheme_count: 1
schemes:
- description: OAuth 2.0 Bearer token. Authenticate via StreamYard's OAuth flow at https://streamyard.com/oauth/authorize.
  flows:
  - authorizationUrl: https://streamyard.com/oauth/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://streamyard.com/oauth/token
  name: streamyardBearerAuth
  sources:
  - openapi/streamyard-openapi.yml
  type: oauth2
slug: streamyard-authentication
source_filename: streamyard-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/streamyard-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: streamyardBearerAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://streamyard.com/oauth/authorize\n    tokenUrl: https://streamyard.com/oauth/token\n    scopes: 3\n  description: OAuth 2.0 Bearer token. Authenticate via StreamYard's OAuth flow at https://streamyard.com/oauth/authorize.\n  sources:\n  - openapi/streamyard-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/streamyard/refs/heads/main/authentication/streamyard-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Broadcasting
- Live Streaming
- Multi-Streaming
- Recordings
- Video
---
