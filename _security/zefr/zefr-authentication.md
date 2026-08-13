---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Zefr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zefr declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Zefr
provider_slug: zefr
scheme_count: 2
schemes:
- description: OpenID Connect 1.0 discovery is served anonymously. Authorization Code with PKCE (S256) is supported, as is the client_credentials grant — the grant a machine-to-machine API client would use.
  id: openIdConnect
  openIdConnectUrl: https://login.zefr.com/.well-known/openid-configuration
  type: openIdConnect
- description: OAuth 2.0 Authorization Server Metadata (RFC 8414) at the same issuer.
  flows:
    authorizationCode:
      authorizationUrl: https://login.zefr.com/authorize
      refreshUrl: https://login.zefr.com/oauth/token
      tokenUrl: https://login.zefr.com/oauth/token
    clientCredentials:
      tokenUrl: https://login.zefr.com/oauth/token
    deviceCode:
      deviceAuthorizationUrl: https://login.zefr.com/oauth/device/code
      tokenUrl: https://login.zefr.com/oauth/token
  id: oauth2
  type: oauth2
slug: zefr-authentication
source_filename: zefr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://login.zefr.com/.well-known/openid-configuration\nnote: >-\n  Zefr publishes no developer portal, no API reference and no OpenAPI, so there is no\n  securityScheme block to derive from. What IS published, anonymously and machine-readably,\n  is the OpenID Connect discovery document for Zefr's own identity provider — an Auth0\n  tenant on the custom domain login.zefr.com (CNAME zefr-prod-cd-qq34zjzlcmyzcxao.edge.tenants.auth0.com)\n  that authenticates the Zefr Brand Suitability Suite at suitability.zefr.com. This profile is\n  read verbatim from that document. It describes how Zefr authenticates identities; it does NOT\n  describe how a customer authenticates against the production API gateway at api.zefr.com,\n  which Zefr does not document publicly.\nissuer: https://login.zefr.com/\nprovider: Auth0 (custom domain)\nschemes:\n- id: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://login.zefr.com/.well-known/openid-configuration\n\
  \  description: >-\n    OpenID Connect 1.0 discovery is served anonymously. Authorization Code with PKCE\n    (S256) is supported, as is the client_credentials grant — the grant a machine-to-machine\n    API client would use.\n- id: oauth2\n  type: oauth2\n  description: OAuth 2.0 Authorization Server Metadata (RFC 8414) at the same issuer.\n  flows:\n    authorizationCode:\n      authorizationUrl: https://login.zefr.com/authorize\n      tokenUrl: https://login.zefr.com/oauth/token\n      refreshUrl: https://login.zefr.com/oauth/token\n    clientCredentials:\n      tokenUrl: https://login.zefr.com/oauth/token\n    deviceCode:\n      deviceAuthorizationUrl: https://login.zefr.com/oauth/device/code\n      tokenUrl: https://login.zefr.com/oauth/token\nendpoints:\n  authorization: https://login.zefr.com/authorize\n  token: https://login.zefr.com/oauth/token\n  userinfo: https://login.zefr.com/userinfo\n  jwks: https://login.zefr.com/.well-known/jwks.json\n  revocation: https://login.zefr.com/oauth/revoke\n\
  \  registration: https://login.zefr.com/oidc/register\n  device_authorization: https://login.zefr.com/oauth/device/code\n  backchannel_authentication: https://login.zefr.com/bc-authorize\n  mfa_challenge: https://login.zefr.com/mfa/challenge\n  global_token_revocation: https://login.zefr.com/oauth/global-token-revocation/connection/{connectionName}\ngrant_types_supported:\n- client_credentials\n- authorization_code\n- refresh_token\n- password\n- implicit\n- urn:ietf:params:oauth:grant-type:device_code\n- urn:ietf:params:oauth:grant-type:token-exchange\n- urn:ietf:params:oauth:grant-type:jwt-bearer\n- http://auth0.com/oauth/grant-type/password-realm\n- http://auth0.com/oauth/grant-type/passwordless/otp\n- http://auth0.com/oauth/grant-type/mfa-oob\n- http://auth0.com/oauth/grant-type/mfa-otp\n- http://auth0.com/oauth/grant-type/mfa-recovery-code\ntoken_endpoint_auth_methods_supported:\n- client_secret_basic\n- client_secret_post\n- private_key_jwt\n- none\npkce:\n  supported: true\n  code_challenge_methods:\n\
  \  - S256\n  - plain\nid_token_signing_alg_values_supported:\n- HS256\n- RS256\n- PS256\ndpop:\n  supported: true\n  signing_alg_values:\n  - ES256\nmfa:\n  supported: true\n  challenge_endpoint: https://login.zefr.com/mfa/challenge\n  note: MFA grant types (mfa-oob, mfa-otp, mfa-recovery-code) are advertised.\nbackchannel_logout:\n  supported: true\n  session_supported: true\ndynamic_client_registration:\n  supported: true\n  endpoint: https://login.zefr.com/oidc/register\n  note: Advertised by the discovery document; not verified (registration was not attempted).\napi_key_auth:\n  documented: false\n  note: >-\n    No public documentation describes an API key, bearer token or signing scheme for\n    api.zefr.com. The gateway (Apigee) answers every anonymous request with a\n    messaging.adaptors.http.flow.ApplicationNotFound fault, so no auth challenge is observable.\ngaps:\n- No public API reference documents how to authenticate against api.zefr.com.\n- No audience/resource identifier\
  \ is published for a Zefr product API.\n- No scope reference page exists; only the standard OIDC identity scopes are advertised.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zefr/refs/heads/main/authentication/zefr-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Adtech
- Brand Safety
- Brand Suitability
- Content Intelligence
- Content Moderation
- Video
- Social Media
- Advertising
- Media Measurement
- Machine Learning
---
