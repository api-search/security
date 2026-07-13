---
api_key_in: []
api_specs:
- filename: warner-music-group-licensing-openapi.yml
  format: yaml
  label: Warner Music Group Licensing API
  slug: wmg-licensing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/warner-music-group/refs/heads/main/openapi/warner-music-group-licensing-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Warner Music Group Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Warner Music Group secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Warner Music Group
provider_slug: warner-music-group
scheme_count: 1
schemes:
- description: OAuth 2.0 for WMG partner authentication
  flows:
  - authorizationUrl: https://auth.wmg.com/oauth/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://auth.wmg.com/oauth/token
  name: OAuth2
  sources:
  - openapi/warner-music-group-licensing-openapi.yml
  type: oauth2
slug: warner-music-group-authentication
source_filename: warner-music-group-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/warner-music-group-licensing-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.wmg.com/oauth/authorize\n    tokenUrl: https://auth.wmg.com/oauth/token\n    scopes: 3\n  description: OAuth 2.0 for WMG partner authentication\n  sources:\n  - openapi/warner-music-group-licensing-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/warner-music-group/refs/heads/main/authentication/warner-music-group-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Music
- Entertainment
- Streaming
- Licensing
- Publishing
---
