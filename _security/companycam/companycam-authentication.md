---
api_key_in: []
api_specs:
- filename: companycam-openapi-original.yml
  format: yaml
  label: CompanyCam Core API (v2)
  slug: companycam-core-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/companycam/refs/heads/main/openapi/companycam-openapi-original.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Companycam Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: CompanyCam secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: CompanyCam
provider_slug: companycam
scheme_count: 2
schemes:
- description: Bearer <API_TOKEN> in the Authorization header. Tokens are minted in-app at https://app.companycam.com/access_tokens or issued via the OAuth flow.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/companycam-openapi-original.yml
  type: http
- description: Authorization-code grant for confidential partner clients. Scopes are space-delimited (read/write/destroy plus per-resource resource:action scopes). See scopes/companycam-scopes.yml.
  flows:
  - authorizationUrl: https://app.companycam.com/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://app.companycam.com/oauth/token
    tokenUrl: https://app.companycam.com/oauth/token
  introspection_endpoint: https://app.companycam.com/oauth/introspect
  name: OAuth2
  pkce: S256
  registration_endpoint: https://app.companycam.com/oauth/register
  revocation_endpoint: https://app.companycam.com/oauth/revoke
  sources:
  - https://app.companycam.com/.well-known/oauth-authorization-server
  - https://docs.companycam.com/docs/oauth
  type: oauth2
slug: companycam-authentication
source_filename: companycam-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/companycam-openapi-original.yml\ndocs: https://docs.companycam.com/docs/getting-started\nsummary:\n  types:\n  - http\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  bearer: true\nnotes: >-\n  Two token paths: (1) a personal access token generated in the CompanyCam app\n  (https://app.companycam.com/access_tokens), sent as an HTTP Bearer token — this\n  is the only scheme declared in the published OpenAPI; (2) full OAuth 2.0\n  authorization-code (with refresh tokens and PKCE S256) for partner integrations,\n  documented separately and advertised at the RFC 8414 authorization-server\n  metadata endpoint. API access requires a Pro, Premium, or Elite plan.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Bearer <API_TOKEN> in the Authorization header. Tokens are minted in-app at\n    https://app.companycam.com/access_tokens or issued via the OAuth flow.\n \
  \ sources:\n  - openapi/companycam-openapi-original.yml\n- name: OAuth2\n  type: oauth2\n  description: >-\n    Authorization-code grant for confidential partner clients. Scopes are\n    space-delimited (read/write/destroy plus per-resource resource:action\n    scopes). See scopes/companycam-scopes.yml.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.companycam.com/oauth/authorize\n    tokenUrl: https://app.companycam.com/oauth/token\n    refreshUrl: https://app.companycam.com/oauth/token\n  pkce: S256\n  revocation_endpoint: https://app.companycam.com/oauth/revoke\n  introspection_endpoint: https://app.companycam.com/oauth/introspect\n  registration_endpoint: https://app.companycam.com/oauth/register\n  sources:\n  - https://app.companycam.com/.well-known/oauth-authorization-server\n  - https://docs.companycam.com/docs/oauth\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/companycam/refs/heads/main/authentication/companycam-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Construction
- Photos
- Field Service
- Project Management
- Contractors
- Documentation
- Webhooks
---
