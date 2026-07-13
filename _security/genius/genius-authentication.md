---
api_key_in: []
api_specs:
- filename: genius-openapi.yml
  format: yaml
  label: Genius
  slug: genius
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genius/refs/heads/main/openapi/genius-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Genius Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Genius secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Genius
provider_slug: genius
scheme_count: 2
schemes:
- description: 'Genius uses OAuth 2.0 with the authorization-code flow. Apps are

    registered at https://genius.com/api-clients.'
  flows:
  - authorizationUrl: https://api.genius.com/oauth/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://api.genius.com/oauth/token
  name: GeniusOAuth2
  sources:
  - openapi/genius-openapi.yml
  type: oauth2
- bearerFormat: client_access_token
  description: 'Client-only access token issued at app registration. Sufficient for

    read-only endpoints (search, songs, artists, albums, annotations,

    referents, web_pages/lookup).'
  name: ClientAccessToken
  scheme: bearer
  sources:
  - openapi/genius-openapi.yml
  type: http
slug: genius-authentication
source_filename: genius-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/genius-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: GeniusOAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.genius.com/oauth/authorize\n    tokenUrl: https://api.genius.com/oauth/token\n    scopes: 4\n  description: |-\n    Genius uses OAuth 2.0 with the authorization-code flow. Apps are\n    registered at https://genius.com/api-clients.\n  sources:\n  - openapi/genius-openapi.yml\n- name: ClientAccessToken\n  type: http\n  scheme: bearer\n  bearerFormat: client_access_token\n  description: |-\n    Client-only access token issued at app registration. Sufficient for\n    read-only endpoints (search, songs, artists, albums, annotations,\n    referents, web_pages/lookup).\n  sources:\n  - openapi/genius-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genius/refs/heads/main/authentication/genius-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Music
- Lyrics
- Annotations
- Crowdsourced
- Reference Data
- Public APIs
---
