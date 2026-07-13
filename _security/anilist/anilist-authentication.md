---
api_key_in: []
api_specs:
- filename: anilist-openapi.yml
  format: yaml
  label: AniList GraphQL API v2
  slug: anilist-graphql-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anilist/refs/heads/main/openapi/anilist-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Anilist Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: AniList secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: AniList
provider_slug: anilist
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: OAuth2 access token issued by AniList. No scopes; access tokens grant (almost) full access to a user's data. Tokens are valid for one year.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/anilist-openapi.yml
  type: http
- description: AniList OAuth2 (no scopes supported)
  flows:
  - authorizationUrl: https://anilist.co/api/v2/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://anilist.co/api/v2/oauth/token
  - authorizationUrl: https://anilist.co/api/v2/oauth/authorize
    flow: implicit
    scopes: 0
  name: oauth2
  sources:
  - openapi/anilist-openapi.yml
  type: oauth2
slug: anilist-authentication
source_filename: anilist-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/anilist-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - implicit\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth2 access token issued by AniList. No scopes; access tokens grant (almost)\n    full access to a user's data. Tokens are valid for one year.\n  sources:\n  - openapi/anilist-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://anilist.co/api/v2/oauth/authorize\n    tokenUrl: https://anilist.co/api/v2/oauth/token\n    scopes: 0\n  - flow: implicit\n    authorizationUrl: https://anilist.co/api/v2/oauth/authorize\n    scopes: 0\n  description: AniList OAuth2 (no scopes supported)\n  sources:\n  - openapi/anilist-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anilist/refs/heads/main/authentication/anilist-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Anime
- Manga
- Entertainment
- Media
- Social
- Database
- GraphQL
- OAuth2
- Public APIs
---
