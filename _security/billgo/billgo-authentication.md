---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Billgo Authentication
name_suffix: Authentication
oauth_flows:
- authorization_code
- implicit
- refresh_token
- password
- device_code
- ciba
overview: BillGO secures its APIs with openIdConnect and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorization_code, implicit, refresh_token, password, device_code, and ciba flow(s).
provider_name: BillGO
provider_slug: billgo
scheme_count: 2
schemes:
- authorization_endpoint: https://exchange-login.billgo.com/oauth2/default/v1/authorize
  code_challenge_methods_supported:
  - S256
  id_token_signing_alg_values_supported:
  - RS256
  introspection_endpoint: https://exchange-login.billgo.com/oauth2/default/v1/introspect
  issuer: https://exchange-login.billgo.com/oauth2/default
  jwks_uri: https://exchange-login.billgo.com/oauth2/default/v1/keys
  name: BillGO Exchange OpenID Connect
  openIdConnectUrl: https://exchange-login.billgo.com/oauth2/default/.well-known/openid-configuration
  registration_endpoint: https://exchange-login.billgo.com/oauth2/v1/clients
  response_types_supported:
  - code
  - id_token
  - code id_token
  - code token
  - id_token token
  - code id_token token
  revocation_endpoint: https://exchange-login.billgo.com/oauth2/default/v1/revoke
  sources:
  - well-known/billgo-openid-configuration.json
  token_endpoint: https://exchange-login.billgo.com/oauth2/default/v1/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - none
  type: openIdConnect
  userinfo_endpoint: https://exchange-login.billgo.com/oauth2/default/v1/userinfo
- grant_types_supported:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - client_credentials
  - urn:ietf:params:oauth:grant-type:device_code
  issuer: https://exchange-login.billgo.com
  metadata: https://exchange-login.billgo.com/.well-known/oauth-authorization-server
  name: Okta org authorization server
  note: This is the stock Okta org authorization server that ships with every Okta tenant. Its scopes are Okta administrative scopes (okta.users.read, okta.apps.manage, ...), not BillGO product scopes. Recorded for completeness; it is not the API's authorization surface.
  sources:
  - well-known/billgo-oauth-authorization-server.json
  type: oauth2
slug: billgo-authentication
source_filename: billgo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-07'\nmethod: probed\nsource: https://exchange-login.billgo.com/oauth2/default/.well-known/openid-configuration\ndocs: https://docs.billgo.com/\ndocs_note: >-\n  The BillGO developer reference is a private ReadMe project — https://docs.billgo.com/\n  returns HTTP 302 to https://dash.readme.com/to/billgo-group for anonymous visitors —\n  so no documented auth page could be read. Everything below is taken from the\n  provider's own anonymously-readable OpenID Connect / OAuth 2.0 discovery documents,\n  not from documentation.\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorization_code\n  - implicit\n  - refresh_token\n  - password\n  - device_code\n  - ciba\n  pkce: true\n  pkce_methods:\n  - S256\n  identity_provider: Okta\nschemes:\n- name: BillGO Exchange OpenID Connect\n  type: openIdConnect\n  openIdConnectUrl: https://exchange-login.billgo.com/oauth2/default/.well-known/openid-configuration\n  issuer:\
  \ https://exchange-login.billgo.com/oauth2/default\n  authorization_endpoint: https://exchange-login.billgo.com/oauth2/default/v1/authorize\n  token_endpoint: https://exchange-login.billgo.com/oauth2/default/v1/token\n  userinfo_endpoint: https://exchange-login.billgo.com/oauth2/default/v1/userinfo\n  jwks_uri: https://exchange-login.billgo.com/oauth2/default/v1/keys\n  registration_endpoint: https://exchange-login.billgo.com/oauth2/v1/clients\n  introspection_endpoint: https://exchange-login.billgo.com/oauth2/default/v1/introspect\n  revocation_endpoint: https://exchange-login.billgo.com/oauth2/default/v1/revoke\n  id_token_signing_alg_values_supported:\n  - RS256\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  - client_secret_jwt\n  - private_key_jwt\n  - none\n  code_challenge_methods_supported:\n  - S256\n  response_types_supported:\n  - code\n  - id_token\n  - code id_token\n  - code token\n  - id_token token\n  - code id_token token\n\
  \  sources:\n  - well-known/billgo-openid-configuration.json\n- name: Okta org authorization server\n  type: oauth2\n  issuer: https://exchange-login.billgo.com\n  metadata: https://exchange-login.billgo.com/.well-known/oauth-authorization-server\n  grant_types_supported:\n  - authorization_code\n  - implicit\n  - refresh_token\n  - password\n  - client_credentials\n  - urn:ietf:params:oauth:grant-type:device_code\n  note: >-\n    This is the stock Okta org authorization server that ships with every Okta tenant.\n    Its scopes are Okta administrative scopes (okta.users.read, okta.apps.manage, ...),\n    not BillGO product scopes. Recorded for completeness; it is not the API's\n    authorization surface.\n  sources:\n  - well-known/billgo-oauth-authorization-server.json\napi_surface:\n  endpoint: https://exchange.billgo.com/graphql\n  transport: GraphQL over HTTPS POST\n  observed:\n    get_method: 405\n    anonymous_typename_query: 200\n    introspection: disabled by the server (IntrospectionDisabled)\n\
  \  bearer_token: >-\n    Not directly observable without credentials. The Exchange SPA is an Apollo client\n    against this endpoint and authenticates through the Okta issuer above, so tokens\n    are OIDC access tokens; the exact header name is not published.\ngaps:\n- No OpenAPI or GraphQL SDL is published, so security schemes cannot be derived from a spec.\n- No public authentication guide; the reference is behind a ReadMe login.\n- No API-key mechanism is documented or observable on any public surface.\nx-evidence:\n  fetched: '2026-08-07'\n  probes:\n  - url: https://exchange-login.billgo.com/oauth2/default/.well-known/openid-configuration\n    status: 200\n  - url: https://exchange-login.billgo.com/.well-known/oauth-authorization-server\n    status: 200\n  - url: https://exchange.billgo.com/graphql\n    status: 200\n    method: POST\n  - url: https://docs.billgo.com/\n    status: 302\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/billgo/refs/heads/main/authentication/billgo-authentication.yml
summary_line: openIdConnect/oauth2 · 2 schemes
tags:
- Payments
- Bill Pay
- Financial-Services
- Banking
- ACH
- Virtual Cards
- Fintech
- GraphQL
---
