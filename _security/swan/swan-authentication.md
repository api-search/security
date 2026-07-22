---
api_key_in: []
auth_types:
- oauth2
- http
description: 'Swan uses OAuth 2.0 (RFC 6749) with Bearer token authentication (RFC 6750). Tokens are supplied in an HTTP Authorization header as `Authorization: Bearer {access token}`. There are two token types: project access tokens (client_credentials grant, project-level access, valid one hour) and user access tokens (authorization_code grant, act on behalf of an individual user, valid one hour, refreshable). A project token can also impersonate a user to perform sensitive mutations. User tokens (and impersonating project tokens) cannot call `transactions` queries.'
kind: authentication
layout: security
method: searched
name: Swan Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
- refreshToken
overview: Swan secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials, authorizationCode, and refreshToken flow(s).
provider_name: Swan
provider_slug: swan
scheme_count: 2
schemes:
- authorization_endpoint: https://oauth.swan.io/oauth2/auth
  code_challenge_methods:
  - S256
  - plain
  flows:
  - flow: clientCredentials
    token_lifetime_seconds: 3600
    use: Project access token (project-level API access)
  - flow: authorizationCode
    refreshable: true
    token_lifetime_seconds: 3600
    use: User access token (act on behalf of a user; required for sensitive mutations)
  grant_types:
  - client_credentials
  - authorization_code
  - refresh_token
  - implicit
  jwks_uri: https://oauth.swan.io/.well-known/jwks.json
  name: OAuth2
  pkce_supported: true
  revocation_endpoint: https://oauth.swan.io/oauth2/revoke
  token_endpoint: https://oauth.swan.io/oauth2/token
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  - none
  type: oauth2
  userinfo_endpoint: https://oauth.swan.io/userinfo
- description: OAuth 2.0 access token presented as a Bearer token to the GraphQL API.
  in: header
  name: BearerAuth
  scheme: bearer
  type: http
slug: swan-authentication
source_filename: swan-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.swan.io/developers/using-api/authentication\ndocs: https://docs.swan.io/developers/using-api/authentication\noidc_discovery: https://oauth.swan.io/.well-known/openid-configuration\nsummary:\n  types: [oauth2, http]\n  http_scheme: bearer\n  oauth2_flows: [clientCredentials, authorizationCode, refreshToken]\ndescription: >-\n  Swan uses OAuth 2.0 (RFC 6749) with Bearer token authentication (RFC 6750).\n  Tokens are supplied in an HTTP Authorization header as\n  `Authorization: Bearer {access token}`. There are two token types: project\n  access tokens (client_credentials grant, project-level access, valid one hour)\n  and user access tokens (authorization_code grant, act on behalf of an\n  individual user, valid one hour, refreshable). A project token can also\n  impersonate a user to perform sensitive mutations. User tokens (and\n  impersonating project tokens) cannot call `transactions` queries.\nschemes:\n- name:\
  \ OAuth2\n  type: oauth2\n  authorization_endpoint: https://oauth.swan.io/oauth2/auth\n  token_endpoint: https://oauth.swan.io/oauth2/token\n  revocation_endpoint: https://oauth.swan.io/oauth2/revoke\n  userinfo_endpoint: https://oauth.swan.io/userinfo\n  jwks_uri: https://oauth.swan.io/.well-known/jwks.json\n  grant_types: [client_credentials, authorization_code, refresh_token, implicit]\n  token_endpoint_auth_methods: [client_secret_post, client_secret_basic, private_key_jwt, none]\n  pkce_supported: true\n  code_challenge_methods: [S256, plain]\n  flows:\n  - flow: clientCredentials\n    use: Project access token (project-level API access)\n    token_lifetime_seconds: 3600\n  - flow: authorizationCode\n    use: User access token (act on behalf of a user; required for sensitive mutations)\n    token_lifetime_seconds: 3600\n    refreshable: true\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  description: OAuth 2.0 access token presented as a Bearer token to the GraphQL\
  \ API.\nnotes: >-\n  Single Device Authentication (a 6-digit SMS verification code) rolled out\n  across all OAuth 2.0 flows starting May 2026, replacing the previous clickable\n  SMS link.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swan/refs/heads/main/authentication/swan-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Banking as a Service
- Embedded Finance
- Fintech
- Payments
- Cards
- SEPA
- GraphQL
- Europe
- Accounts
---
