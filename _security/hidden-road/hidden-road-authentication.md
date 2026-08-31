---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Hidden Road Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hidden Road declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Hidden Road
provider_slug: hidden-road
scheme_count: 2
schemes:
- audience: https://api.hiddenroad.com/v0/
  discovery:
    jwks_uri: https://auth.hiddenroad.com/.well-known/jwks.json
    oauth_authorization_server: https://auth.hiddenroad.com/.well-known/oauth-authorization-server
    openid_configuration: https://auth.hiddenroad.com/.well-known/openid-configuration
  dpop:
    algs:
    - ES256
    supported: true
  endpoints:
    authorization: https://auth.hiddenroad.com/authorize
    backchannel_authentication: https://auth.hiddenroad.com/bc-authorize
    device_authorization: https://auth.hiddenroad.com/oauth/device/code
    end_session: https://auth.hiddenroad.com/oidc/logout
    registration: https://auth.hiddenroad.com/oidc/register
    revocation: https://auth.hiddenroad.com/oauth/revoke
    token: https://auth.hiddenroad.com/oauth/token
    userinfo: https://auth.hiddenroad.com/userinfo
  format: Bearer <JWT>
  grant_types:
  - client_credentials
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - implicit
  - password
  header: Authorization
  id_token_signing_algs:
  - HS256
  - RS256
  - PS256
  in: header
  issuer: https://auth.hiddenroad.com/
  machine_to_machine: true
  machine_to_machine_note: client_credentials is advertised, which is the grant an agent or a treasury system would use against the accountactivity / metrics / atm surfaces.
  mtls: false
  name: hiddenroad_oauth2
  pkce:
    methods:
    - S256
    - plain
    supported: true
  provider: Auth0 (tenant hosted on the company's own auth.hiddenroad.com CNAME)
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: oauth2
- name: hiddenroad_portal_oidc
  openIdConnectUrl: https://auth.hiddenroad.com/.well-known/openid-configuration
  redirect_uri: https://portal.ops.hiddenroad.com/callback
  scopes:
  - openid
  - profile
  - email
  type: openIdConnect
  used_by: https://portal.ops.hiddenroad.com/ (Operational Portal, browser SPA)
slug: hidden-road-authentication
source_filename: hidden-road-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: >-\n  https://auth.hiddenroad.com/.well-known/openid-configuration (HTTP 200) and the unauthenticated\n  JavaScript bundle served by Hidden Road's own Operational Portal at\n  https://portal.ops.hiddenroad.com/assets/index-b9a72e77.js (HTTP 200)\nnote: >-\n  No OpenAPI or public auth reference exists for the Hidden Road API, so this profile was\n  established by probe rather than derived from a spec. Every value below is read verbatim from\n  a first-party Hidden Road host.\nprimary_scheme: oauth2\nschemes:\n- name: hiddenroad_oauth2\n  type: oauth2\n  in: header\n  header: Authorization\n  format: Bearer <JWT>\n  issuer: https://auth.hiddenroad.com/\n  audience: https://api.hiddenroad.com/v0/\n  provider: Auth0 (tenant hosted on the company's own auth.hiddenroad.com CNAME)\n  discovery:\n    openid_configuration: https://auth.hiddenroad.com/.well-known/openid-configuration\n    oauth_authorization_server: https://auth.hiddenroad.com/.well-known/oauth-authorization-server\n\
  \    jwks_uri: https://auth.hiddenroad.com/.well-known/jwks.json\n  endpoints:\n    authorization: https://auth.hiddenroad.com/authorize\n    token: https://auth.hiddenroad.com/oauth/token\n    device_authorization: https://auth.hiddenroad.com/oauth/device/code\n    userinfo: https://auth.hiddenroad.com/userinfo\n    revocation: https://auth.hiddenroad.com/oauth/revoke\n    end_session: https://auth.hiddenroad.com/oidc/logout\n    registration: https://auth.hiddenroad.com/oidc/register\n    backchannel_authentication: https://auth.hiddenroad.com/bc-authorize\n  grant_types:\n  - client_credentials\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - implicit\n  - password\n  machine_to_machine: true\n  machine_to_machine_note: >-\n    client_credentials is advertised, which is the grant an agent or a treasury system would\n    use against the\
  \ accountactivity / metrics / atm surfaces.\n  pkce:\n    supported: true\n    methods: [S256, plain]\n  dpop:\n    supported: true\n    algs: [ES256]\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\n  mtls: false\n  id_token_signing_algs: [HS256, RS256, PS256]\n- name: hiddenroad_portal_oidc\n  type: openIdConnect\n  used_by: https://portal.ops.hiddenroad.com/ (Operational Portal, browser SPA)\n  openIdConnectUrl: https://auth.hiddenroad.com/.well-known/openid-configuration\n  scopes: [openid, profile, email]\n  redirect_uri: https://portal.ops.hiddenroad.com/callback\nobserved_behaviour:\n- url: https://api.hiddenroad.com/v0/accountactivity/ping\n  status: 401\n  body: '{\"message\":\"Unauthorized\"}'\n  meaning: Route exists; bearer token required.\n- url: https://api.hiddenroad.com/v0/openapi.json\n  status: 403\n  body: '{\"message\":\"Missing Authentication Token\"}'\n  meaning: >-\n    AWS API Gateway's response for\
  \ an UNROUTED path. The 401-vs-403 split is what let each\n    real service route be confirmed without credentials.\ncredentials_issuance: >-\n  Not self-serve. Credentials are issued to onboarded institutional counterparties; there is no\n  public signup, sandbox key, or developer registration page.\nweaknesses:\n- No public authentication documentation of any kind.\n- >-\n    The API-level scope vocabulary (otc:read, otc:write, accountactivity:*) is not published\n    anywhere a prospective integrator can read it; it was recovered from the portal bundle.\n- No mutual-TLS option advertised for an institutional prime-brokerage surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hidden-road/refs/heads/main/authentication/hidden-road-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Financial-Services
- Prime Brokerage
- Clearing
- Digital Assets
- Foreign Exchange
- Capital Markets
- Trading
- Institutional Finance
- Collateral Management
- Risk Management
- Regulated
---
