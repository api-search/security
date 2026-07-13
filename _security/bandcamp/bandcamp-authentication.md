---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Bandcamp Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Bandcamp secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Bandcamp
provider_slug: bandcamp
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 access token returned by `/oauth_token`.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/bandcamp-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://bandcamp.com/oauth_token
  name: oauth2
  sources:
  - openapi/bandcamp-openapi.yml
  type: oauth2
slug: bandcamp-authentication
source_filename: bandcamp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bandcamp-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 access token returned by `/oauth_token`.\n  sources:\n  - openapi/bandcamp-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://bandcamp.com/oauth_token\n    scopes: 0\n  sources:\n  - openapi/bandcamp-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bandcamp/refs/heads/main/authentication/bandcamp-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Music
- Marketplace
- Indie
- Audio
- Sales
- Merch
---
