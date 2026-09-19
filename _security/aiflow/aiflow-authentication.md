---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Aiflow Authentication
name_suffix: Authentication
oauth_flows: []
overview: aiFlow declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: aiFlow
provider_slug: aiflow
scheme_count: 2
schemes:
- evidence: https://auth.aiflow.solutions/.well-known/openid-configuration
  in: header
  name: openIdConnect
  openIdConnectUrl: https://auth.aiflow.solutions/.well-known/openid-configuration
  type: openIdConnect
- evidence: https://auth.aiflow.solutions/.well-known/oauth-authorization-server
  flows:
    authorizationCode:
      authorizationUrl: https://auth.aiflow.solutions/authorize
      refreshUrl: https://auth.aiflow.solutions/oauth/token
      tokenUrl: https://auth.aiflow.solutions/oauth/token
    clientCredentials:
      tokenUrl: https://auth.aiflow.solutions/oauth/token
    deviceCode:
      deviceAuthorizationUrl: https://auth.aiflow.solutions/oauth/device/code
      tokenUrl: https://auth.aiflow.solutions/oauth/token
  name: oauth2
  type: oauth2
slug: aiflow-authentication
source_filename: aiflow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: https://auth.aiflow.solutions/.well-known/openid-configuration\ndocs: https://www.veratainsight.com/security\nnote: >-\n  aiFlow publishes no developer API and no API authentication documentation. This profile is read\n  verbatim from the OpenID Connect discovery document the company serves on its own Auth0 custom\n  domain, auth.aiflow.solutions, which is the identity provider for the Verata web application\n  (app.veratainsight.com redirects there to authenticate). It describes END-USER SIGN-IN to the\n  product, not programmatic API access. No API key scheme, bearer-token scheme or developer\n  credential issuance is documented anywhere on either brand's site.\nscope_of_profile: application-sign-in\napi_authentication_documented: false\nissuer: https://auth.aiflow.solutions/\nprovider_stack: Auth0 (custom domain on the company's own registrable domain)\nschemes:\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl:\
  \ https://auth.aiflow.solutions/.well-known/openid-configuration\n  in: header\n  evidence: https://auth.aiflow.solutions/.well-known/openid-configuration\n- name: oauth2\n  type: oauth2\n  flows:\n    authorizationCode:\n      authorizationUrl: https://auth.aiflow.solutions/authorize\n      tokenUrl: https://auth.aiflow.solutions/oauth/token\n      refreshUrl: https://auth.aiflow.solutions/oauth/token\n    clientCredentials:\n      tokenUrl: https://auth.aiflow.solutions/oauth/token\n    deviceCode:\n      deviceAuthorizationUrl: https://auth.aiflow.solutions/oauth/device/code\n      tokenUrl: https://auth.aiflow.solutions/oauth/token\n  evidence: https://auth.aiflow.solutions/.well-known/oauth-authorization-server\nendpoints:\n  authorization: https://auth.aiflow.solutions/authorize\n  token: https://auth.aiflow.solutions/oauth/token\n  userinfo: https://auth.aiflow.solutions/userinfo\n  jwks: https://auth.aiflow.solutions/.well-known/jwks.json\n  revocation: https://auth.aiflow.solutions/oauth/revoke\n\
  \  registration: https://auth.aiflow.solutions/oidc/register\n  device_authorization: https://auth.aiflow.solutions/oauth/device/code\n  backchannel_authentication: https://auth.aiflow.solutions/bc-authorize\n  mfa_challenge: https://auth.aiflow.solutions/mfa/challenge\ngrant_types_supported:\n- client_credentials\n- authorization_code\n- refresh_token\n- password\n- implicit\n- urn:ietf:params:oauth:grant-type:device_code\n- urn:ietf:params:oauth:grant-type:token-exchange\n- urn:ietf:params:oauth:grant-type:jwt-bearer\n- http://auth0.com/oauth/grant-type/password-realm\n- http://auth0.com/oauth/grant-type/passwordless/otp\n- http://auth0.com/oauth/grant-type/mfa-oob\n- http://auth0.com/oauth/grant-type/mfa-otp\n- http://auth0.com/oauth/grant-type/mfa-recovery-code\ntoken_endpoint_auth_methods_supported:\n- client_secret_basic\n- client_secret_post\n- private_key_jwt\n- none\nsecurity_features:\n  pkce: true\n  pkce_methods:\n  - S256\n  - plain\n  dpop: true\n  dpop_signing_alg_values_supported:\n\
  \  - ES256\n  mfa: true\n  dynamic_client_registration: true\n  token_revocation: true\n  global_token_revocation: true\n  id_token_signing_alg_values_supported:\n  - HS256\n  - RS256\n  - PS256\nobserved:\n  live_challenge: >-\n    GET https://app.aiflow.solutions/ 302s to\n    https://auth.aiflow.solutions/authorize with response_type=code, code_challenge_method=S256 and\n    redirect_uri=https://app.veratainsight.com/auth/callback, then to the hosted universal-login page.\n  fetched: '2026-09-14'\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aiflow/refs/heads/main/authentication/aiflow-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Executive Search
- Private Equity
- Talent Intelligence
- People Data
- Company Data
- Market Intelligence
- Artificial Intelligence
- Y Combinator
- No Public API
---
