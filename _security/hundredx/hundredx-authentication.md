---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Hundredx Authentication
name_suffix: Authentication
oauth_flows: []
overview: HundredX declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: HundredX
provider_slug: hundredx
scheme_count: 3
schemes:
- dpop_signing_algs:
  - ES256
  endpoints:
    authorization: https://login.hundredxinc.com/authorize
    backchannel_authentication: https://login.hundredxinc.com/bc-authorize
    device_authorization: https://login.hundredxinc.com/oauth/device/code
    jwks: https://login.hundredxinc.com/.well-known/jwks.json
    registration: https://login.hundredxinc.com/oidc/register
    revocation: https://login.hundredxinc.com/oauth/revoke
    token: https://login.hundredxinc.com/oauth/token
    userinfo: https://login.hundredxinc.com/userinfo
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - implicit
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: hundredx-portal-oidc
  id_token_signing_algs:
  - RS256
  - PS256
  - HS256
  issuer: https://login.hundredxinc.com/
  mfa: true
  mfa_note: mfa_challenge_endpoint present (https://login.hundredxinc.com/mfa/challenge).
  onboarding: invite-only
  onboarding_note: The portal is a customer login, not a signup. Fetching https://portal.hundredx.com/ anonymously redirects to https://login.hundredxinc.com/u/login and returns HTTP 400 without client parameters.
  openIdConnectUrl: https://login.hundredxinc.com/.well-known/openid-configuration
  pkce:
  - S256
  - plain
  provider: Auth0 (custom domain on hundredxinc.com)
  surface: https://portal.hundredx.com/ (HundredX customer insights portal)
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
- authorization_server_metadata:
  - https://hx-bigquery-mcp.hundredx.com/.well-known/oauth-authorization-server
  - https://jupyter-mcp.hundredx.com/.well-known/oauth-authorization-server
  bearer_methods:
  - header
  dynamic_client_registration: true
  grant_types:
  - authorization_code
  - refresh_token
  id: hundredx-mcp-oauth21
  pkce:
  - S256
  - plain
  profile: OAuth 2.1 (MCP authorization), Google-federated identity
  protected_resource_metadata:
  - https://hx-bigquery-mcp.hundredx.com/.well-known/oauth-protected-resource
  - https://jupyter-mcp.hundredx.com/.well-known/oauth-protected-resource
  response_types:
  - code
  surface: https://hx-bigquery-mcp.hundredx.com/mcp and https://jupyter-mcp.hundredx.com/mcp
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
  unauthenticated_response:
    body: '{"error":"invalid_token","error_description":"Missing or invalid access token"}'
    status: 401
- id: hundredx-feedbackhistory-api
  note: A live HAL/Spring HATEOAS API host. Every anonymous request — including /, /v1, /api, /feedback and /profile — returns the same 404 HAL envelope, so no challenge, scheme or realm is exposed. Recorded as unknown rather than guessed.
  surface: https://feedbackhistory.api.hundredxinc.com
  type: unknown
slug: hundredx-authentication
source_filename: hundredx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: >-\n  https://login.hundredxinc.com/.well-known/openid-configuration,\n  https://hx-bigquery-mcp.hundredx.com/.well-known/oauth-authorization-server,\n  https://jupyter-mcp.hundredx.com/.well-known/oauth-authorization-server — all fetched\n  anonymously on 2026-08-22.\nnote: >-\n  Derived from live discovery documents, not from an OpenAPI — HundredX publishes no\n  machine-readable API contract. Every scheme below is the auth in front of a HundredX\n  surface, not a documented developer-facing scheme; HundredX has no public developer\n  program and issues no self-serve credentials.\nschemes:\n  - id: hundredx-portal-oidc\n    surface: https://portal.hundredx.com/ (HundredX customer insights portal)\n    type: openIdConnect\n    openIdConnectUrl: https://login.hundredxinc.com/.well-known/openid-configuration\n    issuer: https://login.hundredxinc.com/\n    provider: Auth0 (custom domain on hundredxinc.com)\n    endpoints:\n  \
  \    authorization: https://login.hundredxinc.com/authorize\n      token: https://login.hundredxinc.com/oauth/token\n      userinfo: https://login.hundredxinc.com/userinfo\n      jwks: https://login.hundredxinc.com/.well-known/jwks.json\n      revocation: https://login.hundredxinc.com/oauth/revoke\n      device_authorization: https://login.hundredxinc.com/oauth/device/code\n      registration: https://login.hundredxinc.com/oidc/register\n      backchannel_authentication: https://login.hundredxinc.com/bc-authorize\n    grant_types:\n      - authorization_code\n      - client_credentials\n      - refresh_token\n      - implicit\n      - password\n      - urn:ietf:params:oauth:grant-type:device_code\n      - urn:ietf:params:oauth:grant-type:token-exchange\n      - urn:ietf:params:oauth:grant-type:jwt-bearer\n    pkce: [S256, plain]\n    token_endpoint_auth_methods: [client_secret_basic, client_secret_post, private_key_jwt, none]\n    id_token_signing_algs: [RS256, PS256, HS256]\n    dpop_signing_algs:\
  \ [ES256]\n    mfa: true\n    mfa_note: mfa_challenge_endpoint present (https://login.hundredxinc.com/mfa/challenge).\n    onboarding: invite-only\n    onboarding_note: >-\n      The portal is a customer login, not a signup. Fetching https://portal.hundredx.com/\n      anonymously redirects to https://login.hundredxinc.com/u/login and returns HTTP 400\n      without client parameters.\n  - id: hundredx-mcp-oauth21\n    surface: https://hx-bigquery-mcp.hundredx.com/mcp and https://jupyter-mcp.hundredx.com/mcp\n    type: oauth2\n    profile: OAuth 2.1 (MCP authorization), Google-federated identity\n    bearer_methods: [header]\n    protected_resource_metadata:\n      - https://hx-bigquery-mcp.hundredx.com/.well-known/oauth-protected-resource\n      - https://jupyter-mcp.hundredx.com/.well-known/oauth-protected-resource\n    authorization_server_metadata:\n      - https://hx-bigquery-mcp.hundredx.com/.well-known/oauth-authorization-server\n      - https://jupyter-mcp.hundredx.com/.well-known/oauth-authorization-server\n\
  \    grant_types: [authorization_code, refresh_token]\n    response_types: [code]\n    pkce: [S256, plain]\n    dynamic_client_registration: true\n    token_endpoint_auth_methods: [client_secret_basic, client_secret_post, none]\n    unauthenticated_response:\n      status: 401\n      body: '{\"error\":\"invalid_token\",\"error_description\":\"Missing or invalid access token\"}'\n  - id: hundredx-feedbackhistory-api\n    surface: https://feedbackhistory.api.hundredxinc.com\n    type: unknown\n    note: >-\n      A live HAL/Spring HATEOAS API host. Every anonymous request — including /, /v1, /api,\n      /feedback and /profile — returns the same 404 HAL envelope, so no challenge, scheme or\n      realm is exposed. Recorded as unknown rather than guessed.\napi_keys: none_published\napi_keys_note: HundredX publishes no API key issuance, key prefix, or credential documentation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hundredx/refs/heads/main/authentication/hundredx-authentication.yml
summary_line: 3 schemes
tags:
- customer-experience
- consumer-insights
- market-research
- alternative-data
- investment-research
- data-licensing
---
