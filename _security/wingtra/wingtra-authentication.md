---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: probed
name: Wingtra Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wingtra declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Wingtra
provider_slug: wingtra
scheme_count: 3
schemes:
- authorization_endpoint: https://my-wingtra.eu.auth0.com/authorize
  discovery: https://my-wingtra.eu.auth0.com/.well-known/openid-configuration
  dynamic_registration:
    endpoint: https://my-wingtra.eu.auth0.com/oidc/register
    note: Advertised in the discovery document. Advertisement is not an invitation — Wingtra does not offer third-party API clients, and this endpoint was not exercised.
  flow: authorization_code with PKCE (S256)
  grant_types:
  - authorization_code
  - refresh_token
  - client_credentials
  - password
  - implicit
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: auth0-oidc
  id_token_signing_algs:
  - RS256
  - PS256
  - HS256
  issuer: https://my-wingtra.eu.auth0.com/
  jwks_uri: https://my-wingtra.eu.auth0.com/.well-known/jwks.json
  mfa: The tenant advertises /mfa/challenge and the mfa-oob, mfa-otp and mfa-recovery-code grants, so MFA is available; whether it is enforced for a given Wingtra account is not observable anonymously.
  pkce_methods:
  - S256
  - plain
  revocation_endpoint: https://my-wingtra.eu.auth0.com/oauth/revoke
  scopes: scopes/wingtra-scopes.yml
  surfaces:
  - portal.wingtra.com
  - my.wingtra.com
  - cloud.wingtra.com
  token_endpoint: https://my-wingtra.eu.auth0.com/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
  userinfo_endpoint: https://my-wingtra.eu.auth0.com/userinfo
- bearer_format: JWT
  detail: The schema's `login` mutation returns LoginResponse { access_token, refresh_token, token_type, expires_in, scope, assigned_roles, user_info }, and `refreshToken` renews it — an OAuth-shaped envelope handed back over GraphQL. Authenticated calls carry the access token as a bearer credential. The User type mirrors an Auth0 profile (user_id, identities[].provider, app_metadata.tenantId), which is what ties this API to the Auth0 tenant above.
  id: portal-graphql-bearer
  roles:
    field: assigned_roles
    note: Role names are returned per user; no public list of roles is published.
  scheme: bearer
  surface: https://api.my.wingtra.com/graphql
  type: http
- detail: Not determinable anonymously. Every unauthenticated request to this host, including the /v1 paths its own web client calls, is answered HTTP 400 "Something went wrong." by an edge in front of the application — not 401, not WWW-Authenticate. The schema's `getSkyToken` query and the client's Auth0 session together indicate a bearer token minted from the same tenant, but no anonymous probe confirms the scheme, so it is recorded as unknown rather than assumed.
  id: sky-rest-unknown
  surface: https://api.sky.wingtra.com
  type: unknown
slug: wingtra-authentication
source_filename: wingtra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource:\n- https://my-wingtra.eu.auth0.com/.well-known/openid-configuration\n- https://portal.wingtra.com/\n- https://api.my.wingtra.com/graphql\n- graphql/wingtra-my-portal.graphql\ndocs: null\nsummary: >-\n  Wingtra publishes no authentication documentation for developers, because it issues no\n  developer credentials. Everything below was established by probing surfaces that answer\n  anonymously. Human sign-in across the Wingtra estate is Auth0 — the tenant\n  my-wingtra.eu.auth0.com, named by portal.wingtra.com's own 302 to\n  /authorize?client_id=...&scope=openid%20profile%20email&response_type=code with PKCE\n  S256. Machine access to the portal GraphQL API is a bearer access token minted by that\n  tenant, or by the API's own `login` mutation, which returns an OAuth-shaped token\n  envelope directly.\nschemes:\n- id: auth0-oidc\n  type: openIdConnect\n  surfaces: [portal.wingtra.com, my.wingtra.com, cloud.wingtra.com]\n  issuer:\
  \ https://my-wingtra.eu.auth0.com/\n  discovery: https://my-wingtra.eu.auth0.com/.well-known/openid-configuration\n  authorization_endpoint: https://my-wingtra.eu.auth0.com/authorize\n  token_endpoint: https://my-wingtra.eu.auth0.com/oauth/token\n  userinfo_endpoint: https://my-wingtra.eu.auth0.com/userinfo\n  revocation_endpoint: https://my-wingtra.eu.auth0.com/oauth/revoke\n  jwks_uri: https://my-wingtra.eu.auth0.com/.well-known/jwks.json\n  flow: authorization_code with PKCE (S256)\n  pkce_methods: [S256, plain]\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - client_credentials\n  - password\n  - implicit\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  id_token_signing_algs: [RS256, PS256, HS256]\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, private_key_jwt, none]\n  mfa: >-\n    The tenant advertises /mfa/challenge and the mfa-oob, mfa-otp\
  \ and mfa-recovery-code\n    grants, so MFA is available; whether it is enforced for a given Wingtra account is not\n    observable anonymously.\n  dynamic_registration:\n    endpoint: https://my-wingtra.eu.auth0.com/oidc/register\n    note: >-\n      Advertised in the discovery document. Advertisement is not an invitation — Wingtra\n      does not offer third-party API clients, and this endpoint was not exercised.\n  scopes: scopes/wingtra-scopes.yml\n- id: portal-graphql-bearer\n  type: http\n  scheme: bearer\n  surface: https://api.my.wingtra.com/graphql\n  bearer_format: JWT\n  detail: >-\n    The schema's `login` mutation returns LoginResponse { access_token, refresh_token,\n    token_type, expires_in, scope, assigned_roles, user_info }, and `refreshToken` renews\n    it — an OAuth-shaped envelope handed back over GraphQL. Authenticated calls carry the\n    access token as a bearer credential. The User type mirrors an Auth0 profile\n    (user_id, identities[].provider, app_metadata.tenantId),\
  \ which is what ties this API\n    to the Auth0 tenant above.\n  roles:\n    field: assigned_roles\n    note: Role names are returned per user; no public list of roles is published.\n- id: sky-rest-unknown\n  type: unknown\n  surface: https://api.sky.wingtra.com\n  detail: >-\n    Not determinable anonymously. Every unauthenticated request to this host, including the\n    /v1 paths its own web client calls, is answered HTTP 400 \"Something went wrong.\" by an\n    edge in front of the application — not 401, not WWW-Authenticate. The schema's\n    `getSkyToken` query and the client's Auth0 session together indicate a bearer token\n    minted from the same tenant, but no anonymous probe confirms the scheme, so it is\n    recorded as unknown rather than assumed.\nanonymous_access:\n  graphql_introspection:\n    open: true\n    endpoint: https://api.my.wingtra.com/graphql\n    verified: '2026-09-04'\n    http_status: 200\n    detail: >-\n      __schema answers unauthenticated callers in full.\
  \ Field resolvers were NOT exercised;\n      only the introspection meta-field was queried. This is a posture finding worth\n      reporting to Wingtra — production GraphQL services normally disable introspection —\n      and it is the only reason this repository can describe the API at all.\n  cors:\n    access_control_allow_origin: '*'\n    access_control_allow_credentials: 'true'\n    note: >-\n      Observed on the live 200. `*` together with allow-credentials is a combination\n      browsers reject, so it is recorded as observed rather than interpreted.\nfindings_for_provider:\n- Anonymous GraphQL introspection is enabled on the production api.my.wingtra.com endpoint.\n- No security.txt is served on any Wingtra host, so there is no published route for the above.\nx-evidence:\n  fetched: '2026-09-04'\n  probes:\n  - {url: 'https://my-wingtra.eu.auth0.com/.well-known/openid-configuration', http_status: 200}\n  - {url: 'https://portal.wingtra.com/', http_status: 302, note: 'redirects\
  \ to my-wingtra.eu.auth0.com/authorize'}\n  - {url: 'https://api.my.wingtra.com/graphql', http_status: 200, note: 'anonymous introspection succeeded'}\n  - {url: 'https://api.sky.wingtra.com/v1/sites', http_status: 400}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wingtra/refs/heads/main/authentication/wingtra-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Drones
- UAV
- Aerial Surveying
- Mapping
- Photogrammetry
- Geospatial
- Surveying
- LiDAR
- Hardware
- Switzerland
---
