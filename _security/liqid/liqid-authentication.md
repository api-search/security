---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Liqid Authentication
name_suffix: Authentication
oauth_flows: []
overview: LIQID Investments declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: LIQID Investments
provider_slug: liqid
scheme_count: 0
schemes: []
slug: liqid-authentication
source_filename: liqid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: https://authentication.liqid.de/.well-known/openid-configuration\nscope_note: >-\n  LIQID publishes no developer API, so there is no third-party authentication model to\n  document. What follows is the authentication surface LIQID actually serves anonymously:\n  the OpenID Connect discovery metadata of the identity providers that front its own\n  customer applications. Nothing here grants an external developer access; it is recorded\n  because it is the only machine-readable auth contract the company publishes.\nproviders:\n- name: LIQID customer login\n  host: authentication.liqid.de\n  platform: Auth0 (custom domain; tenant liqid.eu.auth0.com)\n  discovery: https://authentication.liqid.de/.well-known/openid-configuration\n  discovery_http_status: 200\n  rfc8414_authorization_server_metadata: https://authentication.liqid.de/.well-known/oauth-authorization-server\n  rfc8414_http_status: 200\n  file: well-known/liqid-authentication-openid-configuration.json\n\
  \  issuer: https://authentication.liqid.de/\n  endpoints:\n    authorization: https://authentication.liqid.de/authorize\n    token: https://authentication.liqid.de/oauth/token\n    userinfo: https://authentication.liqid.de/userinfo\n    jwks: https://authentication.liqid.de/.well-known/jwks.json\n    revocation: https://authentication.liqid.de/oauth/revoke\n    registration: https://authentication.liqid.de/oidc/register\n    device_authorization: https://authentication.liqid.de/oauth/device/code\n    backchannel_authentication: https://authentication.liqid.de/bc-authorize\n    mfa_challenge: https://authentication.liqid.de/mfa/challenge\n  schemes:\n  - type: openIdConnect\n    id: liqid-oidc\n    detail: OpenID Connect 1.0 discovery document served anonymously.\n  - type: oauth2\n    id: liqid-oauth2-authorization-code\n    flow: authorizationCode\n    pkce: true\n    pkce_methods:\n    - S256\n    - plain\n  - type: oauth2\n    id: liqid-oauth2-client-credentials\n    flow: clientCredentials\n\
  \  - type: oauth2\n    id: liqid-oauth2-device-code\n    flow: deviceCode\n    grant: urn:ietf:params:oauth:grant-type:device_code\n  grant_types_supported:\n  - client_credentials\n  - authorization_code\n  - refresh_token\n  - password\n  - implicit\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\n  id_token_signing_algs:\n  - HS256\n  - RS256\n  - PS256\n  dpop_signing_algs:\n  - ES256\n  mfa: true\n  mfa_detail: >-\n    An mfa_challenge_endpoint is advertised and Auth0 MFA grant types\n    (mfa-oob, mfa-otp, mfa-recovery-code) are supported.\n  backchannel_logout: true\n- name: LIQID client portal\n  host: app.liqid.de\n  platform: Salesforce Experience Cloud on a LIQID domain\n  discovery: https://app.liqid.de/.well-known/openid-configuration\n  discovery_http_status:\
  \ 200\n  file: well-known/liqid-app-openid-configuration.json\n  issuer: https://app.liqid.de\n  note: >-\n    Served from a host LIQID controls, but the document describes the Salesforce\n    platform's OAuth surface (scopes_supported are Salesforce platform scopes such as\n    cdp_query_api, wave_api and pardot_api), not a LIQID-designed API.\n  schemes:\n  - type: openIdConnect\n    id: liqid-app-oidc\n  - type: oauth2\n    id: liqid-app-oauth2\n    flow: authorizationCode\napplication_api:\n  host: api.liqid.de\n  documented: false\n  http_status_unauthenticated: 401\n  body_unauthenticated: '{\"message\":\"unauthorized\"}'\n  health_endpoint: https://api.liqid.de/health\n  health_http_status: 200\n  note: >-\n    LIQID's own application API answers 401 with a JSON envelope on every path probed\n    (/, /docs, /redoc, /api-docs, /v1, /openapi, /graphql, /mcp, /.well-known/*). Only\n    /health responds anonymously. No scheme, header name or token format is published,\n    so the authentication\
  \ model for this API is undocumented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liqid/refs/heads/main/authentication/liqid-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Wealth Management
- Investing
- Financial Services
- Private Equity
- Venture Capital
- Asset Management
- Fintech
- Germany
- BaFin
---
