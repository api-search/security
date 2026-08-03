---
api_key_in: []
api_specs:
- filename: 1komma5-offer-tool-openapi-original.json
  format: json
  label: 1KOMMA5° Offer Tool API
  slug: 1komma5-offer-tool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1komma5/refs/heads/main/openapi/1komma5-offer-tool-openapi-original.json
auth_types:
- openIdConnect
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: 1Komma5 Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- implicit
- password
- deviceCode
- refreshToken
- tokenExchange
- jwtBearer
overview: 1KOMMA5° secures its APIs with openIdConnect, oauth2, and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, implicit, password, deviceCode, refreshToken, tokenExchange, and jwtBearer flow(s).
provider_name: 1KOMMA5°
provider_slug: 1komma5
scheme_count: 3
schemes:
- backchannel_logout_supported: true
  code_challenge_methods_supported:
  - S256
  - plain
  dpop_signing_alg_values_supported:
  - ES256
  dynamic_client_registration: true
  endpoints:
    authorization: https://auth.1komma5grad.com/authorize
    backchannel_authentication: https://auth.1komma5grad.com/bc-authorize
    device_authorization: https://auth.1komma5grad.com/oauth/device/code
    global_token_revocation: https://auth.1komma5grad.com/oauth/global-token-revocation/connection/{connectionName}
    jwks: https://auth.1komma5grad.com/.well-known/jwks.json
    mfa_challenge: https://auth.1komma5grad.com/mfa/challenge
    registration: https://auth.1komma5grad.com/oidc/register
    revocation: https://auth.1komma5grad.com/oauth/revoke
    token: https://auth.1komma5grad.com/oauth/token
    userinfo: https://auth.1komma5grad.com/userinfo
  id_token_signing_alg_values_supported:
  - HS256
  - RS256
  - PS256
  issuer: https://auth.1komma5grad.com/
  name: auth0-oidc
  openIdConnectUrl: https://auth.1komma5grad.com/.well-known/openid-configuration
  provider: Auth0
  response_modes_supported:
  - query
  - fragment
  - form_post
  sources:
  - well-known/1komma5-openid-configuration.json
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
- applied_to:
  - SendOfferController_sendOffer_v1
  - RefreshConfigEnergySiteInfoController_refresh_v1
  name: bearer
  note: Declared in operation-level `security` and backed by a required `authorization` header parameter, but there is no matching entry under components.securitySchemes in the published spec. Recorded as observed, not invented.
  scheme: bearer
  sources:
  - openapi/1komma5-offer-tool-openapi-original.json
  status: referenced-but-undefined
  type: http
- applies_to: https://heartbeat.1komma5grad.com
  flows:
  - authorizationUrl: https://auth.1komma5grad.com/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://auth.1komma5grad.com/oauth/token
  name: heartbeat-oauth2-pkce
  note: The Heartbeat customer API is gated by the same Auth0 tenant. 1KOMMA5° documents no client credentials or developer onboarding path for it; the mobile-app flow (authorization code + PKCE) is what community clients replicate.
  sources:
  - well-known/1komma5-openid-configuration.json
  status: undocumented
  type: oauth2
slug: 1komma5-authentication
source_filename: 1komma5-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://auth.1komma5grad.com/.well-known/openid-configuration\ndocs: null\nnote: >-\n  1KOMMA5° publishes no developer authentication documentation. This profile was built\n  from two real, anonymously-fetchable sources: the Auth0 OIDC discovery document at\n  auth.1komma5grad.com, and the live Offer Tool OpenAPI. Note the Offer Tool spec is\n  DEFECTIVE for auth — `components.securitySchemes` is absent (null) even though two\n  operations carry `security: [{bearer: []}]` and declare a required `authorization`\n  header parameter. The scheme named `bearer` is therefore referenced but never defined.\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  - http\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  - password\n  - deviceCode\n  - refreshToken\n  - tokenExchange\n  - jwtBearer\n  pkce: true\n  mfa: true\n  dpop: true\nschemes:\n- name: auth0-oidc\n  type: openIdConnect\n\
  \  openIdConnectUrl: https://auth.1komma5grad.com/.well-known/openid-configuration\n  issuer: https://auth.1komma5grad.com/\n  provider: Auth0\n  endpoints:\n    authorization: https://auth.1komma5grad.com/authorize\n    token: https://auth.1komma5grad.com/oauth/token\n    userinfo: https://auth.1komma5grad.com/userinfo\n    jwks: https://auth.1komma5grad.com/.well-known/jwks.json\n    revocation: https://auth.1komma5grad.com/oauth/revoke\n    registration: https://auth.1komma5grad.com/oidc/register\n    device_authorization: https://auth.1komma5grad.com/oauth/device/code\n    backchannel_authentication: https://auth.1komma5grad.com/bc-authorize\n    mfa_challenge: https://auth.1komma5grad.com/mfa/challenge\n    global_token_revocation: https://auth.1komma5grad.com/oauth/global-token-revocation/connection/{connectionName}\n  id_token_signing_alg_values_supported:\n  - HS256\n  - RS256\n  - PS256\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n\
  \  - private_key_jwt\n  - none\n  code_challenge_methods_supported:\n  - S256\n  - plain\n  response_modes_supported:\n  - query\n  - fragment\n  - form_post\n  dpop_signing_alg_values_supported:\n  - ES256\n  backchannel_logout_supported: true\n  dynamic_client_registration: true\n  sources:\n  - well-known/1komma5-openid-configuration.json\n- name: bearer\n  type: http\n  scheme: bearer\n  status: referenced-but-undefined\n  applied_to:\n  - SendOfferController_sendOffer_v1\n  - RefreshConfigEnergySiteInfoController_refresh_v1\n  note: >-\n    Declared in operation-level `security` and backed by a required `authorization`\n    header parameter, but there is no matching entry under components.securitySchemes\n    in the published spec. Recorded as observed, not invented.\n  sources:\n  - openapi/1komma5-offer-tool-openapi-original.json\n- name: heartbeat-oauth2-pkce\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    pkce: S256\n    authorizationUrl: https://auth.1komma5grad.com/authorize\n\
  \    tokenUrl: https://auth.1komma5grad.com/oauth/token\n  applies_to: https://heartbeat.1komma5grad.com\n  status: undocumented\n  note: >-\n    The Heartbeat customer API is gated by the same Auth0 tenant. 1KOMMA5° documents\n    no client credentials or developer onboarding path for it; the mobile-app flow\n    (authorization code + PKCE) is what community clients replicate.\n  sources:\n  - well-known/1komma5-openid-configuration.json\ngaps:\n- Offer Tool OpenAPI declares no components.securitySchemes — the `bearer` scheme it\n  references is undefined, so tooling cannot resolve auth from the spec.\n- No public developer registration, API key issuance, or partner onboarding page found\n  for either API.\n- No documented scope model for the Offer Tool API; authorization appears to be\n  role/tenant based (Admin - Roles, Tenants, branches) rather than scope based.\nx-evidence:\n  fetched: '2026-08-02'\n  urls:\n  - url: https://auth.1komma5grad.com/.well-known/openid-configuration\n\
  \    http_status: 200\n    content_type: application/json\n  - url: https://api.offer.1komma5grad.com/swagger-json\n    http_status: 200\n    content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1komma5/refs/heads/main/authentication/1komma5-authentication.yml
summary_line: openIdConnect/oauth2/http · 3 schemes
tags:
- Company
- Energy
- Solar
- Renewable Energy
- Smart Home
- Electric Vehicles
- Heat Pumps
- Virtual Power Plant
- Energy Management
- Germany
---
