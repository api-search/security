---
api_key_in: []
api_specs:
- filename: basis-analytics-api-openapi.yml
  format: yaml
  label: Basis Analytics API
  slug: basis-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basis/refs/heads/main/openapi/basis-analytics-api-openapi.yml
auth_types:
- oauth2
- http
description: 'Every Basis Platform API endpoint requires authentication. Basis uses OAuth 2.0 with an Auth0-hosted authorization server at https://auth.basis.net — explicitly NOT the API host. Access tokens are presented to https://api.basis.net as `Authorization: Bearer <access_token>`. Credentials are not self-serve: the API is available to Basis (formerly Centro) customers and integration partners, and organizations must obtain credentials from their Basis representative.'
kind: authentication
layout: security
method: searched
name: Basis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Basis secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Basis
provider_slug: basis
scheme_count: 2
schemes:
- flows:
  - audience: https://api.basis.net
    authorization_endpoint: https://auth.basis.net/authorize
    grant: authorization_code
    note: The only flow that returns a refresh token. Requires a redirect URI registered with Basis support.
    pkce: supported (code_challenge_methods_supported S256, plain)
    scopes:
    - openid
    - profile
    - email
    - offline_access
    token_endpoint: https://auth.basis.net/oauth/token
  - audience: https://api.basis.net
    grant: client_credentials
    note: Machine-to-machine. The application must have an associated owner (agency) ID or the token endpoint returns 401. The resulting token covers all clients for that agency, so Basis recommends the authorization-code flow where restricted clients exist. User-scoped endpoints (e.g. GET /v1/me) return 404 under this flow because the token represents an organization, not a user.
    quota:
      exhausted_status: 429
      tokens_per_day: 25
      tokens_per_hour: 10
    token_endpoint: https://auth.basis.net/oauth/token
  - grant: refresh_token
    note: Returns a new access token and a new refresh token.
    token_endpoint: https://auth.basis.net/oauth/token
  name: OAuth2
  note: Declared in the OpenAPI as a bare securityScheme with no `flows` object; the flows below are documented in prose in the same specification's info.description and confirmed against the authorization server's discovery document.
  sources:
  - openapi/basis-analytics-api-openapi.yml
  type: oauth2
- example: 'curl -X GET "https://api.basis.net/v1/agency" -H "Authorization: Bearer <access_token>"'
  header: 'Authorization: Bearer <access_token>'
  name: Bearer
  scheme: bearer
  sources:
  - openapi/basis-analytics-api-openapi.yml
  type: http
slug: basis-authentication
source_filename: basis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  Authentication section of the Basis Platform API description published by Basis\n  at https://api.basis.net/swagger.json (fetched 2026-08-13, HTTP 200), plus the\n  authorization-server discovery document at\n  https://auth.basis.net/.well-known/openid-configuration (HTTP 200). Scheme names\n  derived from openapi/basis-analytics-api-openapi.yml.\ndocs: https://api.basis.net/swagger.json\ndescription: >-\n  Every Basis Platform API endpoint requires authentication. Basis uses OAuth 2.0\n  with an Auth0-hosted authorization server at https://auth.basis.net — explicitly\n  NOT the API host. Access tokens are presented to https://api.basis.net as\n  `Authorization: Bearer <access_token>`. Credentials are not self-serve: the API\n  is available to Basis (formerly Centro) customers and integration partners, and\n  organizations must obtain credentials from their Basis representative.\nsummary:\n  types:\n    - oauth2\n   \
  \ - http\n  primary: oauth2\n  self_serve_credentials: false\nschemes:\n  - name: OAuth2\n    type: oauth2\n    sources:\n      - openapi/basis-analytics-api-openapi.yml\n    note: >-\n      Declared in the OpenAPI as a bare securityScheme with no `flows` object; the\n      flows below are documented in prose in the same specification's\n      info.description and confirmed against the authorization server's discovery\n      document.\n    flows:\n      - grant: authorization_code\n        authorization_endpoint: https://auth.basis.net/authorize\n        token_endpoint: https://auth.basis.net/oauth/token\n        audience: https://api.basis.net\n        scopes: [openid, profile, email, offline_access]\n        pkce: supported (code_challenge_methods_supported S256, plain)\n        note: >-\n          The only flow that returns a refresh token. Requires a redirect URI\n          registered with Basis support.\n      - grant: client_credentials\n        token_endpoint: https://auth.basis.net/oauth/token\n\
  \        audience: https://api.basis.net\n        note: >-\n          Machine-to-machine. The application must have an associated owner\n          (agency) ID or the token endpoint returns 401. The resulting token\n          covers all clients for that agency, so Basis recommends the\n          authorization-code flow where restricted clients exist. User-scoped\n          endpoints (e.g. GET /v1/me) return 404 under this flow because the token\n          represents an organization, not a user.\n        quota:\n          tokens_per_hour: 10\n          tokens_per_day: 25\n          exhausted_status: 429\n      - grant: refresh_token\n        token_endpoint: https://auth.basis.net/oauth/token\n        note: Returns a new access token and a new refresh token.\n  - name: Bearer\n    type: http\n    scheme: bearer\n    sources:\n      - openapi/basis-analytics-api-openapi.yml\n    header: 'Authorization: Bearer <access_token>'\n    example: 'curl -X GET \"https://api.basis.net/v1/agency\" -H\
  \ \"Authorization: Bearer <access_token>\"'\ndeprecated:\n  - grant: password\n    status: deprecated\n    evidence: >-\n      \"The password grant flow has now been deprecated. Please update your\n      applications to use one of the above two flows.\" — Basis Platform API\n      description, https://api.basis.net/swagger.json\n    note: >-\n      The authorization server still advertises `password` and\n      `http://auth0.com/oauth/grant-type/password-realm` in\n      grant_types_supported, but Basis's own documentation deprecates it for this\n      API.\ntoken_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\nid_token_signing_alg_values_supported: [HS256, RS256, PS256]\ndpop_signing_alg_values_supported: [ES256]\nunauthenticated_behavior:\n  status: 401\n  body: '{\"message\":\"missing authorization header\"}'\n  evidence: probed https://api.basis.net/v1/me on 2026-08-13 (HTTP 401)\nrelated:\n  - scopes/basis-scopes.yml\n\
  \  - well-known/basis-openid-configuration.json\n  - conventions/basis-conventions.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/basis/refs/heads/main/authentication/basis-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Programmatic Advertising
- DSP
- Media Buying
- Campaign Management
- Audience Targeting
- AdTech
---
