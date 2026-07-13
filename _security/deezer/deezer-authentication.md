---
api_key_in: []
api_specs:
- filename: deezer-openapi.yml
  format: yaml
  label: Deezer API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deezer/refs/heads/main/openapi/deezer-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Deezer Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Deezer secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Deezer
provider_slug: deezer
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://connect.deezer.com/oauth/auth.php
    flow: authorizationCode
    scopes: 7
    tokenUrl: https://connect.deezer.com/oauth/access_token.php
  name: oauth2
  sources:
  - openapi/deezer-openapi.yml
  type: oauth2
slug: deezer-authentication
source_filename: deezer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/deezer-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://connect.deezer.com/oauth/auth.php\n    tokenUrl: https://connect.deezer.com/oauth/access_token.php\n    scopes: 7\n  sources:\n  - openapi/deezer-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deezer/refs/heads/main/authentication/deezer-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Music
- Streaming
- Audio
- OAuth
- Catalog
- Playlists
---
