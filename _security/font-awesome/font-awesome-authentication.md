---
api_key_in:
- header
auth_types:
- http
- bearer
- token-exchange
description: ''
kind: authentication
layout: security
method: searched
name: Font Awesome Authentication
name_suffix: Authentication
oauth_flows: []
overview: Font Awesome secures its APIs with http, bearer, and token-exchange across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Font Awesome
provider_slug: font-awesome
scheme_count: 2
schemes:
- description: Long-lived API token created from the Font Awesome account dashboard. Exchanged (not used directly on GraphQL requests) for an access token.
  format: Bearer <API_TOKEN>
  in: header
  name: apiToken
  parameter: Authorization
  type: apiKey
  where: POST https://api.fontawesome.com/token
- bearerFormat: JWT
  description: Short-lived JWT returned by the token endpoint; carries the granted scopes and is sent on GraphQL requests that access authorized fields.
  expires_in: 3600
  format: Bearer <ACCESS_TOKEN>
  in: header
  name: accessToken
  parameter: Authorization
  scheme: bearer
  type: http
  where: POST https://api.fontawesome.com (GraphQL)
slug: font-awesome-authentication
source_filename: font-awesome-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.fontawesome.com/apis/graphql/token-endpoint\ndocs: https://docs.fontawesome.com/apis/graphql/auth\nsummary:\n  types: [http, bearer, token-exchange]\n  api_key_in: [header]\n  public_access: true\nmodel: >-\n  The Font Awesome GraphQL API is public by default — most schema fields require\n  no authorization. Protected fields (account, Kits, Pro SVG data, entitlements)\n  require a bearer access token. An account-generated API token is POSTed to the\n  token endpoint, which returns a short-lived (3600s) JWT access token whose\n  scopes are inherited from the API token.\nschemes:\n  - name: apiToken\n    type: apiKey\n    in: header\n    parameter: Authorization\n    format: \"Bearer <API_TOKEN>\"\n    where: POST https://api.fontawesome.com/token\n    description: >-\n      Long-lived API token created from the Font Awesome account dashboard.\n      Exchanged (not used directly on GraphQL requests) for an access\
  \ token.\n  - name: accessToken\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    in: header\n    parameter: Authorization\n    format: \"Bearer <ACCESS_TOKEN>\"\n    where: POST https://api.fontawesome.com (GraphQL)\n    expires_in: 3600\n    description: >-\n      Short-lived JWT returned by the token endpoint; carries the granted scopes\n      and is sent on GraphQL requests that access authorized fields.\ntoken_endpoint:\n  url: https://api.fontawesome.com/token\n  method: POST\n  request: 'Authorization: Bearer <API_TOKEN>'\n  response_fields: [access_token, token_type, scopes, expires_in]\ngraphql_endpoint: https://api.fontawesome.com\nscopes_ref: scopes/font-awesome-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/font-awesome/refs/heads/main/authentication/font-awesome-authentication.yml
summary_line: http/bearer/token-exchange · 2 schemes
tags:
- Icons
- SVG
- Fonts
- Web Design
- Developer Tools
- GraphQL
- Icon Library
- Frontend
- Design System
- Company
---
