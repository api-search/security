---
api_key_in: []
api_specs:
- filename: ibotta-products-api-openapi.yml
  format: yaml
  label: Ibotta Products API
  slug: ibotta-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibotta/refs/heads/main/openapi/ibotta-products-api-openapi.yml
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Ibotta Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- deviceCode
- refreshToken
overview: Ibotta secures its APIs with http, oauth2, and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, deviceCode, and refreshToken flow(s).
provider_name: Ibotta
provider_slug: ibotta
scheme_count: 2
schemes:
- applies_to: Ibotta Product API (https://api.ibops.net/bex-api)
  description: 'Service-level bearer token. Ibotta''s own plugin manifest declares auth.type "service_http" with authorization_type "bearer" and has_user_authentication false — i.e. a single shared service credential, not per-user auth. Tokens are not self-serve; there is no published key-issuance flow. Verified live on 2026-08-12: an anonymous POST to /openai/search returns HTTP 401 with {"message":"Unauthorized"}.'
  name: bearerAuth
  scheme: bearer
  self_serve: false
  sources:
  - well-known/ibotta-ai-plugin.json
  - openapi/ibotta-product-api-openapi.yml
  type: http
- applies_to: Ibotta Performance Network partner portal (https://portal.ipn.ibotta.com/)
  description: Auth0 tenant at auth.dashboard.ibotta.com. dashboard.ibotta.com 301s to portal.ipn.ibotta.com, which 307s every unauthenticated request to /api/auth/login?returnTo=... and on into the tenant's universal login. Discovery metadata, including JWKS, is served anonymously; the portal contents are not.
  dpop_signing_algs:
  - ES256
  endpoints:
    authorization: https://auth.dashboard.ibotta.com/authorize
    backchannel_authentication: https://auth.dashboard.ibotta.com/bc-authorize
    device_authorization: https://auth.dashboard.ibotta.com/oauth/device/code
    jwks: https://auth.dashboard.ibotta.com/.well-known/jwks.json
    registration: https://auth.dashboard.ibotta.com/oidc/register
    revocation: https://auth.dashboard.ibotta.com/oauth/revoke
    token: https://auth.dashboard.ibotta.com/oauth/token
    userinfo: https://auth.dashboard.ibotta.com/userinfo
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - password
  - implicit
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_algs:
  - HS256
  - RS256
  - PS256
  issuer: https://auth.dashboard.ibotta.com/
  mfa: Tenant exposes /mfa/challenge plus mfa-oob, mfa-otp and mfa-recovery-code grant types — MFA is configurable for partner portal accounts.
  name: ipnPortalOidc
  openid_connect_url: https://auth.dashboard.ibotta.com/.well-known/openid-configuration
  pkce:
  - S256
  - plain
  see: scopes/ibotta-scopes.yml
  sources:
  - well-known/ibotta-dashboard-openid-configuration.json
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
slug: ibotta-authentication
source_filename: ibotta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: >-\n  https://ibotta.com/.well-known/ai-plugin.json (auth block) +\n  https://auth.dashboard.ibotta.com/.well-known/openid-configuration +\n  openapi/ibotta-product-api-openapi.yml + live 401 observed on\n  POST https://api.ibops.net/bex-api/openai/search\ndocs: https://ipn.ibotta.com/integrating-with-the-ipn\nsummary:\n  types:\n  - http\n  - oauth2\n  - openIdConnect\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - deviceCode\n  - refreshToken\n  note: >-\n    Two distinct auth surfaces. (1) The public Ibotta Product API uses a service-level HTTP\n    bearer token. (2) The IPN partner portal is fronted by an Auth0 tenant that publishes full\n    OIDC/RFC 8414 discovery metadata anonymously. The IPN partner APIs themselves are documented\n    only inside that portal, so their authentication scheme is not publicly verifiable.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n\
  \  applies_to: Ibotta Product API (https://api.ibops.net/bex-api)\n  description: >-\n    Service-level bearer token. Ibotta's own plugin manifest declares\n    auth.type \"service_http\" with authorization_type \"bearer\" and\n    has_user_authentication false — i.e. a single shared service credential, not per-user auth.\n    Tokens are not self-serve; there is no published key-issuance flow. Verified live on\n    2026-08-12: an anonymous POST to /openai/search returns HTTP 401 with\n    {\"message\":\"Unauthorized\"}.\n  self_serve: false\n  sources:\n  - well-known/ibotta-ai-plugin.json\n  - openapi/ibotta-product-api-openapi.yml\n- name: ipnPortalOidc\n  type: openIdConnect\n  applies_to: Ibotta Performance Network partner portal (https://portal.ipn.ibotta.com/)\n  openid_connect_url: https://auth.dashboard.ibotta.com/.well-known/openid-configuration\n  description: >-\n    Auth0 tenant at auth.dashboard.ibotta.com. dashboard.ibotta.com 301s to\n    portal.ipn.ibotta.com, which 307s\
  \ every unauthenticated request to\n    /api/auth/login?returnTo=... and on into the tenant's universal login. Discovery metadata,\n    including JWKS, is served anonymously; the portal contents are not.\n  issuer: https://auth.dashboard.ibotta.com/\n  endpoints:\n    authorization: https://auth.dashboard.ibotta.com/authorize\n    token: https://auth.dashboard.ibotta.com/oauth/token\n    userinfo: https://auth.dashboard.ibotta.com/userinfo\n    jwks: https://auth.dashboard.ibotta.com/.well-known/jwks.json\n    registration: https://auth.dashboard.ibotta.com/oidc/register\n    revocation: https://auth.dashboard.ibotta.com/oauth/revoke\n    device_authorization: https://auth.dashboard.ibotta.com/oauth/device/code\n    backchannel_authentication: https://auth.dashboard.ibotta.com/bc-authorize\n  grant_types:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - password\n  - implicit\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n\
  \  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  pkce:\n  - S256\n  - plain\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\n  id_token_signing_algs:\n  - HS256\n  - RS256\n  - PS256\n  dpop_signing_algs:\n  - ES256\n  mfa: >-\n    Tenant exposes /mfa/challenge plus mfa-oob, mfa-otp and mfa-recovery-code grant types —\n    MFA is configurable for partner portal accounts.\n  see: scopes/ibotta-scopes.yml\n  sources:\n  - well-known/ibotta-dashboard-openid-configuration.json\ngaps:\n- The Ibotta Performance Network partner APIs (offer ingestion, redemption, anti-stacking) have\n  no public authentication documentation; the technical reference lives inside the gated portal.\n- No public key-issuance, key-rotation, or credential-scoping documentation for the Product API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ibotta/refs/heads/main/authentication/ibotta-authentication.yml
summary_line: http/oauth2/openIdConnect · 2 schemes
tags:
- Company
- Consumer
- Cashback
- Rewards
- Retail Media
- Coupons
- Loyalty
- Shopping
- Advertising
- Promotions
- Product Search
- Retail
- Affiliates
- CPG
---
