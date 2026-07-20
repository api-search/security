---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Firework Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Firework secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Firework
provider_slug: firework
scheme_count: 2
schemes:
- flow: clientCredentials
  name: OAuth2 Client Credentials
  note: Server-to-server flow documented for the Public API (/api/v1/*). OAuth apps (client_id / client_secret) are registered and scoped to a business by the Firework IS (Internal Systems) team; credentials can only access resources belonging to that business. Not self-service.
  sources:
  - docs.firework.com/firework-for-developers/api/authentication
  token_endpoint: https://api.firework.com/oauth/token
  type: oauth2
- authorization_endpoint: https://api.firework.com/oauth/authorize
  code_challenge_methods:
  - S256
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  name: OAuth2 Authorization Code (PKCE)
  registration_endpoint: https://api.firework.com/oauth/register
  revocation_endpoint: https://api.firework.com/oauth/revoke
  sources:
  - well-known/firework-oauth-authorization-server.json
  token_endpoint: https://api.firework.com/oauth/token
  type: oauth2
slug: firework-authentication
source_filename: firework-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.firework.com/firework-for-developers/api/authentication.md\ndocs: https://docs.firework.com/firework-for-developers/api/authentication\nwell_known: well-known/firework-oauth-authorization-server.json\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials, authorizationCode]\n  token_endpoint_auth_methods: [none, client_secret_post, client_secret_basic]\n  pkce: S256\n  dynamic_client_registration: true       # RFC 7591 registration_endpoint\n  token_revocation: true                   # RFC 7009 revocation_endpoint\n  base_url: https://api.firework.com\n  api_prefix: /api/v1/\nschemes:\n  - name: OAuth2 Client Credentials\n    type: oauth2\n    flow: clientCredentials\n    token_endpoint: https://api.firework.com/oauth/token\n    note: >-\n      Server-to-server flow documented for the Public API (/api/v1/*). OAuth apps\n      (client_id / client_secret) are registered and scoped to a business by the\n\
  \      Firework IS (Internal Systems) team; credentials can only access resources\n      belonging to that business. Not self-service.\n    sources: [docs.firework.com/firework-for-developers/api/authentication]\n  - name: OAuth2 Authorization Code (PKCE)\n    type: oauth2\n    flow: authorizationCode\n    authorization_endpoint: https://api.firework.com/oauth/authorize\n    token_endpoint: https://api.firework.com/oauth/token\n    revocation_endpoint: https://api.firework.com/oauth/revoke\n    registration_endpoint: https://api.firework.com/oauth/register\n    code_challenge_methods: [S256]\n    grant_types: [authorization_code, refresh_token]\n    sources: [well-known/firework-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/firework/refs/heads/main/authentication/firework-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Consumer
- Video Commerce
- Shoppable Video
- Livestream Shopping
- Ecommerce
- Retail
- Video
- SDK
- Webhooks
---
