---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Annexus Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Annexus Health declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Annexus Health
provider_slug: annexus-health
scheme_count: 0
schemes: []
slug: annexus-health-authentication
source_filename: annexus-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: https://login.live.annexushealth.com/.well-known/openid-configuration\ndocs: https://www.annexushealth.com/privacy-security/\nsummary: >-\n  Annexus Health fronts the AssistPoint platform with an OpenID Connect / OAuth 2.0\n  authorization server on its own custom domain, login.live.annexushealth.com. The discovery\n  document is served anonymously and is the only machine-readable authentication contract the\n  company publishes; the AssistPoint business API it protects is partner-gated and has no\n  public reference. The tenant is Auth0-hosted, evidenced by the Auth0-namespaced grant types\n  (http://auth0.com/oauth/grant-type/*) and the /mfa/challenge endpoint in the discovery\n  document.\nissuer: https://login.live.annexushealth.com/\nsecurity_schemes:\n- name: assistpoint_oidc\n  type: openIdConnect\n  openIdConnectUrl: https://login.live.annexushealth.com/.well-known/openid-configuration\n  description: >-\n    OpenID\
  \ Connect Discovery 1.0 metadata for the AssistPoint production identity tier.\n- name: assistpoint_oauth2\n  type: oauth2\n  flows:\n    authorizationCode:\n      authorizationUrl: https://login.live.annexushealth.com/authorize\n      tokenUrl: https://login.live.annexushealth.com/oauth/token\n      refreshUrl: https://login.live.annexushealth.com/oauth/token\n      scopes_ref: scopes/annexus-health-scopes.yml\n    clientCredentials:\n      tokenUrl: https://login.live.annexushealth.com/oauth/token\n      scopes_ref: scopes/annexus-health-scopes.yml\n    deviceCode:\n      deviceAuthorizationUrl: https://login.live.annexushealth.com/oauth/device/code\n      tokenUrl: https://login.live.annexushealth.com/oauth/token\nendpoints:\n  authorization: https://login.live.annexushealth.com/authorize\n  token: https://login.live.annexushealth.com/oauth/token\n  userinfo: https://login.live.annexushealth.com/userinfo\n  jwks: https://login.live.annexushealth.com/.well-known/jwks.json\n  registration:\
  \ https://login.live.annexushealth.com/oidc/register\n  revocation: https://login.live.annexushealth.com/oauth/revoke\n  device_authorization: https://login.live.annexushealth.com/oauth/device/code\n  mfa_challenge: https://login.live.annexushealth.com/mfa/challenge\n  backchannel_authentication: https://login.live.annexushealth.com/bc-authorize\n  global_token_revocation: https://login.live.annexushealth.com/oauth/global-token-revocation/connection/{connectionName}\ngrant_types:\n- client_credentials\n- authorization_code\n- refresh_token\n- password\n- implicit\n- urn:ietf:params:oauth:grant-type:device_code\n- urn:ietf:params:oauth:grant-type:token-exchange\n- urn:ietf:params:oauth:grant-type:jwt-bearer\n- http://auth0.com/oauth/grant-type/password-realm\n- http://auth0.com/oauth/grant-type/passwordless/otp\n- http://auth0.com/oauth/grant-type/mfa-oob\n- http://auth0.com/oauth/grant-type/mfa-otp\n- http://auth0.com/oauth/grant-type/mfa-recovery-code\nclient_authentication:\n- client_secret_basic\n\
  - client_secret_post\n- private_key_jwt\n- none\ntoken_signing:\n  id_token_alg_values: [HS256, RS256, PS256]\n  token_endpoint_auth_signing_alg_values: [RS256, RS384, PS256]\n  dpop_signing_alg_values: [ES256]\nhardening:\n  pkce: true\n  pkce_methods: [S256, plain]\n  pkce_plain_still_offered: true\n  dpop: true\n  mfa: true\n  dynamic_client_registration: true\n  backchannel_logout: true\n  backchannel_logout_session: true\n  token_revocation: true\n  request_object_support: false\n  request_uri_support: false\n  private_key_jwt: true\nobservations:\n- >-\n  Both S256 and plain are advertised as PKCE challenge methods; plain offers no protection\n  against an authorization-code interception attack and is only present for legacy clients.\n- >-\n  The deprecated ROPC (password) and implicit grants remain enabled alongside the modern\n  authorization_code + PKCE and client_credentials grants.\n- >-\n  HS256 is advertised for ID token signing alongside RS256/PS256; symmetric ID token signing\n\
  \  is discouraged for public clients.\n- >-\n  No per-API resource scopes are advertised — the fourteen advertised scopes are the standard\n  OIDC profile set. Any AssistPoint / AP Connect resource scopes are issued per partner and\n  are not published.\nx-evidence:\n  fetched: '2026-08-06'\n  url: https://login.live.annexushealth.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json; charset=utf-8\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/annexus-health/refs/heads/main/authentication/annexus-health-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Healthcare
- Health Technology
- Patient Access
- Financial Assistance
- Oncology
- Revenue Cycle
- Copay Assistance
- Identity
- OpenID Connect
- HITRUST
---
