---
api_key_in:
- header
auth_types:
- http
- oauth2
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Tuum Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
- tokenExchange
overview: Tuum secures its APIs with http, oauth2, and mutualTLS across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, refreshToken, and tokenExchange flow(s).
provider_name: Tuum
provider_slug: tuum
scheme_count: 2
schemes:
- description: JSON Web Token obtained from POST /api/v1/authorise (Auth API) using assigned employee/API-user credentials; refreshed via POST /api/v1/authorise/refresh. Presented as the x-auth-token header.
  in: header
  name: TuumJwt
  parameter_name: x-auth-token
  reference: https://developer.tuumplatform.com/explore#auth-api_post_/api/v1/authorise
  refresh_endpoint: https://[api-name].[environment].tuumplatform.com/api/v1/authorise/refresh
  sources:
  - docs
  token_endpoint: https://[api-name].[environment].tuumplatform.com/api/v1/authorise
  type: apiKey
- authorization_endpoint: https://auth-api.sandbox.tuumplatform.com/oauth2/authorize
  description: RFC 8414 OAuth 2.0 authorization server advertised at /.well-known/oauth-authorization-server on the auth-api host.
  dpop: true
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - urn:ietf:params:oauth:grant-type:token-exchange
  introspection_endpoint: https://auth-api.sandbox.tuumplatform.com/oauth2/introspect
  issuer: https://auth-api.sandbox.tuumplatform.com
  jwks_uri: https://auth-api.sandbox.tuumplatform.com/oauth2/jwks
  mtls_bound_access_tokens: true
  name: TuumOAuth2
  pkce:
  - S256
  revocation_endpoint: https://auth-api.sandbox.tuumplatform.com/oauth2/revoke
  source: well-known/tuum-oauth-authorization-server.json
  sources:
  - well-known
  token_endpoint: https://auth-api.sandbox.tuumplatform.com/oauth2/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - tls_client_auth
  - self_signed_tls_client_auth
  type: oauth2
slug: tuum-authentication
source_filename: tuum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.tuum.com/tuum-developer-docs/getting-started/api-call-essentials/authentication-and-token-refresh.md\ndocs: https://docs.tuum.com/tuum-developer-docs/getting-started/api-call-essentials\nsummary:\n  types: [http, oauth2, mutualTLS]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken, tokenExchange]\n  notes: >-\n    Two coexisting models. (1) The primary/legacy Tuum API auth is a proprietary\n    JWT scheme: authenticate with username + password against the Auth API to\n    receive a JSON Web Token, then present it in the custom x-auth-token request\n    header on every subsequent call. (2) The auth-api host also runs a standards\n    OAuth 2.0 / RFC 8414 authorization server (used for OAuth2 client-credentials\n    webhook delivery and modern integrations) supporting PKCE, DPoP, mTLS-bound\n    tokens, and token exchange.\nschemes:\n  - name: TuumJwt\n    type: apiKey\n\
  \    in: header\n    parameter_name: x-auth-token\n    description: >-\n      JSON Web Token obtained from POST /api/v1/authorise (Auth API) using\n      assigned employee/API-user credentials; refreshed via\n      POST /api/v1/authorise/refresh. Presented as the x-auth-token header.\n    token_endpoint: https://[api-name].[environment].tuumplatform.com/api/v1/authorise\n    refresh_endpoint: https://[api-name].[environment].tuumplatform.com/api/v1/authorise/refresh\n    reference: https://developer.tuumplatform.com/explore#auth-api_post_/api/v1/authorise\n    sources: [docs]\n  - name: TuumOAuth2\n    type: oauth2\n    description: >-\n      RFC 8414 OAuth 2.0 authorization server advertised at\n      /.well-known/oauth-authorization-server on the auth-api host.\n    issuer: https://auth-api.sandbox.tuumplatform.com\n    authorization_endpoint: https://auth-api.sandbox.tuumplatform.com/oauth2/authorize\n    token_endpoint: https://auth-api.sandbox.tuumplatform.com/oauth2/token\n    jwks_uri:\
  \ https://auth-api.sandbox.tuumplatform.com/oauth2/jwks\n    introspection_endpoint: https://auth-api.sandbox.tuumplatform.com/oauth2/introspect\n    revocation_endpoint: https://auth-api.sandbox.tuumplatform.com/oauth2/revoke\n    grant_types: [authorization_code, client_credentials, refresh_token, 'urn:ietf:params:oauth:grant-type:token-exchange']\n    token_endpoint_auth_methods: [client_secret_basic, client_secret_post, client_secret_jwt, private_key_jwt, tls_client_auth, self_signed_tls_client_auth]\n    pkce: [S256]\n    dpop: true\n    mtls_bound_access_tokens: true\n    source: well-known/tuum-oauth-authorization-server.json\n    sources: [well-known]\nwebhook_authentication:\n  # Options Tuum applies to OUTBOUND webhook requests so your receiver can verify them.\n  source: https://docs.tuum.com/tuum-developer-docs/getting-started/notification-api/webhooks/webhook-security-options.md\n  options:\n    - bearer-token\n    - custom-auth-header\n    - oauth2-client-credentials\n  \
  \  - hmac-signature\n    - mtls\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tuum/refs/heads/main/authentication/tuum-authentication.yml
summary_line: http/oauth2/mutualTLS · 2 schemes
tags:
- Company
- Core Banking
- Banking as a Service
- Payments
- Lending
- Cards
- Fintech
- Financial Services
- API
---
