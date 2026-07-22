---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Smashgg Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Smashgg secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Smashgg
provider_slug: smashgg
scheme_count: 2
schemes:
- creation: https://start.gg developer settings ("Create new token")
  docs: https://developer.start.gg/docs/authentication
  expiry: 1 year
  format: 'Authorization: Bearer [token]'
  header: Authorization
  in: header
  name: PersonalAccessToken
  notes: Copy the token immediately on creation - it is not shown again.
  scheme: bearer
  type: http
- docs: https://developer.start.gg/docs/oauth/oauth-overview
  flows:
  - access_token_ttl_seconds: 604800
    authorizationUrl: https://start.gg/oauth/authorize
    flow: authorizationCode
    refresh: true
    scopes:
    - user.identity
    - user.email
    - tournament.manager
    - tournament.reporter
    tokenUrl: https://api.start.gg/oauth/access_token
    token_type: Bearer
  name: OAuth2
  type: oauth2
slug: smashgg-authentication
source_filename: smashgg-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.start.gg/docs/authentication\ndocs: https://developer.start.gg/docs/authentication\nsummary:\n  types: [http, oauth2]\n  http_scheme: bearer\n  oauth2_flows: [authorizationCode]\n  notes: >-\n    start.gg's GraphQL API accepts two token types. A personal access token\n    (created in Developer Settings, expires after 1 year) authenticates\n    application-owned requests. OAuth 2.0 authorization-code tokens act on\n    behalf of an end user, scoped to what the user approves.\nschemes:\n  - name: PersonalAccessToken\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: 'Authorization: Bearer [token]'\n    creation: https://start.gg developer settings (\"Create new token\")\n    expiry: 1 year\n    notes: Copy the token immediately on creation - it is not shown again.\n    docs: https://developer.start.gg/docs/authentication\n  - name: OAuth2\n    type: oauth2\n    flows:\n\
  \      - flow: authorizationCode\n        authorizationUrl: https://start.gg/oauth/authorize\n        tokenUrl: https://api.start.gg/oauth/access_token\n        refresh: true\n        access_token_ttl_seconds: 604800\n        token_type: Bearer\n        scopes:\n          - user.identity\n          - user.email\n          - tournament.manager\n          - tournament.reporter\n    docs: https://developer.start.gg/docs/oauth/oauth-overview\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smashgg/refs/heads/main/authentication/smashgg-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Consumer
- Esports
- Gaming
- Tournaments
- GraphQL
- Events
- Developer API
---
