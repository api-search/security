---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Darrow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Darrow declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Darrow
provider_slug: darrow
scheme_count: 4
schemes:
- description: OpenID Connect discovery for the Darrow customer portal.
  id: openIdConnect
  openIdConnectUrl: https://auth.darrow.ai/.well-known/openid-configuration
  type: openIdConnect
- authorizationUrl: https://auth.darrow.ai/authorize
  description: Interactive login for portal.darrow.ai / platform.darrow.ai.
  flow: authorizationCode
  id: oauth2_authorization_code
  pkce: true
  pkce_methods:
  - S256
  - plain
  refreshUrl: https://auth.darrow.ai/oauth/token
  tokenUrl: https://auth.darrow.ai/oauth/token
  type: oauth2
- description: Advertised by the tenant's grant_types_supported. Machine-to-machine credentials are not offered publicly; issuance would be a tenant/contract matter.
  flow: clientCredentials
  id: oauth2_client_credentials
  tokenUrl: https://auth.darrow.ai/oauth/token
  type: oauth2
- deviceAuthorizationUrl: https://auth.darrow.ai/oauth/device/code
  flow: deviceCode
  id: oauth2_device_code
  tokenUrl: https://auth.darrow.ai/oauth/token
  type: oauth2
slug: darrow-authentication
source_filename: darrow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: https://auth.darrow.ai/.well-known/openid-configuration\ndocs: null\nnote: >-\n  Darrow publishes no public API reference, so this profile is derived entirely from the\n  OpenID Connect discovery document its Auth0 tenant serves anonymously. It describes how\n  the Darrow customer portal authenticates users — it is NOT a published developer\n  authentication scheme, and no API key, client-credential issuance flow or token\n  documentation is available to the public.\nissuer: https://auth.darrow.ai/\nprovider: Auth0 (tenant also reachable at https://darrow.us.auth0.com/)\nschemes:\n- id: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://auth.darrow.ai/.well-known/openid-configuration\n  description: OpenID Connect discovery for the Darrow customer portal.\n- id: oauth2_authorization_code\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://auth.darrow.ai/authorize\n  tokenUrl: https://auth.darrow.ai/oauth/token\n\
  \  refreshUrl: https://auth.darrow.ai/oauth/token\n  pkce: true\n  pkce_methods:\n  - S256\n  - plain\n  description: Interactive login for portal.darrow.ai / platform.darrow.ai.\n- id: oauth2_client_credentials\n  type: oauth2\n  flow: clientCredentials\n  tokenUrl: https://auth.darrow.ai/oauth/token\n  description: >-\n    Advertised by the tenant's grant_types_supported. Machine-to-machine credentials\n    are not offered publicly; issuance would be a tenant/contract matter.\n- id: oauth2_device_code\n  type: oauth2\n  flow: deviceCode\n  deviceAuthorizationUrl: https://auth.darrow.ai/oauth/device/code\n  tokenUrl: https://auth.darrow.ai/oauth/token\nendpoints:\n  authorization: https://auth.darrow.ai/authorize\n  token: https://auth.darrow.ai/oauth/token\n  userinfo: https://auth.darrow.ai/userinfo\n  jwks: https://auth.darrow.ai/.well-known/jwks.json\n  revocation: https://auth.darrow.ai/oauth/revoke\n  registration: https://auth.darrow.ai/oidc/register\n  device_authorization: https://auth.darrow.ai/oauth/device/code\n\
  \  backchannel_authentication: https://auth.darrow.ai/bc-authorize\n  mfa_challenge: https://auth.darrow.ai/mfa/challenge\n  global_token_revocation: https://auth.darrow.ai/oauth/global-token-revocation/connection/{connectionName}\ngrant_types_supported:\n- client_credentials\n- authorization_code\n- refresh_token\n- password\n- implicit\n- urn:ietf:params:oauth:grant-type:device_code\n- urn:ietf:params:oauth:grant-type:token-exchange\n- urn:ietf:params:oauth:grant-type:jwt-bearer\n- http://auth0.com/oauth/grant-type/password-realm\n- http://auth0.com/oauth/grant-type/passwordless/otp\n- http://auth0.com/oauth/grant-type/mfa-oob\n- http://auth0.com/oauth/grant-type/mfa-otp\n- http://auth0.com/oauth/grant-type/mfa-recovery-code\ntoken_endpoint_auth_methods_supported:\n- client_secret_basic\n- client_secret_post\n- private_key_jwt\n- none\nid_token_signing_alg_values_supported:\n- HS256\n- RS256\n- PS256\nfeatures:\n  pkce: true\n  dpop: true\n  dpop_signing_alg_values_supported:\n  - ES256\n\
  \  dynamic_client_registration: true\n  mfa: true\n  ciba_backchannel: true\n  token_exchange: true\n  request_parameter_supported: false\n  request_uri_parameter_supported: false\nobservations:\n- The tenant still advertises the legacy `password` and `implicit` grants alongside\n  authorization_code + PKCE; both are discouraged by OAuth 2.1.\n- HS256 remains in id_token_signing_alg_values_supported, so a symmetric-signed ID token\n  is possible for clients configured that way.\n- No /.well-known/oauth-protected-resource document is served (404), so there is no\n  published resource-server metadata binding an API audience to this issuer.\nx-evidence:\n  fetched: '2026-08-11'\n  url: https://auth.darrow.ai/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/darrow/refs/heads/main/authentication/darrow-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Legal
- Legal Intelligence
- Litigation
- Artificial Intelligence
- Compliance
- Risk Management
- Insurance
- Data Analytics
---
