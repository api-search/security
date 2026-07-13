---
api_key_in: []
api_specs:
- filename: restream-openapi.yml
  format: yaml
  label: Restream API
  slug: restream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restream/refs/heads/main/openapi/restream-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Restream Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Restream secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Restream
provider_slug: restream
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://api.restream.io/oauth/authorize
    flow: authorizationCode
    scopes: 7
    tokenUrl: https://api.restream.io/oauth/token
  name: OAuth2
  sources:
  - openapi/restream-openapi.yml
  type: oauth2
slug: restream-authentication
source_filename: restream-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/restream-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.restream.io/oauth/authorize\n    tokenUrl: https://api.restream.io/oauth/token\n    scopes: 7\n  sources:\n  - openapi/restream-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/restream/refs/heads/main/authentication/restream-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Broadcast
- Chat
- Content Delivery
- Live Streaming
- Multistreaming
- Video Streaming
---
