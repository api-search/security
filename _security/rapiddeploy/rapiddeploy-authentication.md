---
api_key_in: []
auth_types: []
description: RapidDeploy publishes no API reference and no OpenAPI securitySchemes, so this profile is built entirely from the anonymous OpenID Connect / RFC 8414 discovery documents served by the company's own Auth0 tenant at auth.rapiddeploy.com (issuer https://auth.rapiddeploy.com/). Everything below was read out of that document; nothing is inferred from marketing copy.
kind: authentication
layout: security
method: probed
name: Rapiddeploy Authentication
name_suffix: Authentication
oauth_flows: []
overview: RapidDeploy declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: RapidDeploy
provider_slug: rapiddeploy
scheme_count: 4
schemes:
- authorization_url: https://auth.rapiddeploy.com/authorize
  flow: authorizationCode
  id: oauth2_authorization_code
  note: Interactive agency/user sign-in for the RapidDeploy web applications.
  pkce: true
  pkce_methods:
  - S256
  - plain
  token_url: https://auth.rapiddeploy.com/oauth/token
  type: oauth2
- flow: clientCredentials
  id: oauth2_client_credentials
  note: client_credentials is advertised in grant_types_supported, which is the machine-to-machine path an integrator would use against api.rapiddeploy.com. No public documentation describes the audience value or how credentials are issued - that is a tenant/partner process.
  token_url: https://auth.rapiddeploy.com/oauth/token
  type: oauth2
- device_authorization_url: https://auth.rapiddeploy.com/oauth/device/code
  flow: deviceCode
  id: oauth2_device_code
  token_url: https://auth.rapiddeploy.com/oauth/token
  type: oauth2
- id: openIdConnect
  issuer: https://auth.rapiddeploy.com/
  jwks_uri: https://auth.rapiddeploy.com/.well-known/jwks.json
  openid_connect_url: https://auth.rapiddeploy.com/.well-known/openid-configuration
  type: openIdConnect
  userinfo_endpoint: https://auth.rapiddeploy.com/userinfo
slug: rapiddeploy-authentication
source_filename: rapiddeploy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://auth.rapiddeploy.com/.well-known/openid-configuration\ndocs: null\nname: RapidDeploy authentication profile\ndescription: >-\n  RapidDeploy publishes no API reference and no OpenAPI securitySchemes, so this profile is built\n  entirely from the anonymous OpenID Connect / RFC 8414 discovery documents served by the company's\n  own Auth0 tenant at auth.rapiddeploy.com (issuer https://auth.rapiddeploy.com/). Everything below\n  was read out of that document; nothing is inferred from marketing copy.\nprovider_hosts:\n  api: https://api.rapiddeploy.com\n  identity: https://auth.rapiddeploy.com\nschemes:\n- id: oauth2_authorization_code\n  type: oauth2\n  flow: authorizationCode\n  authorization_url: https://auth.rapiddeploy.com/authorize\n  token_url: https://auth.rapiddeploy.com/oauth/token\n  pkce: true\n  pkce_methods:\n  - S256\n  - plain\n  note: 'Interactive agency/user sign-in for the RapidDeploy web applications.'\n\
  - id: oauth2_client_credentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://auth.rapiddeploy.com/oauth/token\n  note: >-\n    client_credentials is advertised in grant_types_supported, which is the machine-to-machine path\n    an integrator would use against api.rapiddeploy.com. No public documentation describes the\n    audience value or how credentials are issued - that is a tenant/partner process.\n- id: oauth2_device_code\n  type: oauth2\n  flow: deviceCode\n  device_authorization_url: https://auth.rapiddeploy.com/oauth/device/code\n  token_url: https://auth.rapiddeploy.com/oauth/token\n- id: openIdConnect\n  type: openIdConnect\n  openid_connect_url: https://auth.rapiddeploy.com/.well-known/openid-configuration\n  issuer: https://auth.rapiddeploy.com/\n  userinfo_endpoint: https://auth.rapiddeploy.com/userinfo\n  jwks_uri: https://auth.rapiddeploy.com/.well-known/jwks.json\ngrant_types_supported:\n- client_credentials\n- authorization_code\n- refresh_token\n-\
  \ password\n- implicit\n- urn:ietf:params:oauth:grant-type:device_code\n- urn:ietf:params:oauth:grant-type:token-exchange\n- urn:ietf:params:oauth:grant-type:jwt-bearer\n- http://auth0.com/oauth/grant-type/password-realm\n- http://auth0.com/oauth/grant-type/passwordless/otp\n- http://auth0.com/oauth/grant-type/mfa-oob\n- http://auth0.com/oauth/grant-type/mfa-otp\n- http://auth0.com/oauth/grant-type/mfa-recovery-code\ntoken_endpoint_auth_methods_supported:\n- client_secret_basic\n- client_secret_post\n- private_key_jwt\n- none\ntoken_signing:\n  id_token_signing_alg_values_supported:\n  - HS256\n  - RS256\n  - PS256\n  token_endpoint_auth_signing_alg_values_supported:\n  - RS256\n  - RS384\n  - PS256\n  dpop_signing_alg_values_supported:\n  - ES256\nendpoints:\n  authorization: https://auth.rapiddeploy.com/authorize\n  token: https://auth.rapiddeploy.com/oauth/token\n  userinfo: https://auth.rapiddeploy.com/userinfo\n  revocation: https://auth.rapiddeploy.com/oauth/revoke\n  registration:\
  \ https://auth.rapiddeploy.com/oidc/register\n  device_authorization: https://auth.rapiddeploy.com/oauth/device/code\n  mfa_challenge: https://auth.rapiddeploy.com/mfa/challenge\n  backchannel_authentication: https://auth.rapiddeploy.com/bc-authorize\n  jwks: https://auth.rapiddeploy.com/.well-known/jwks.json\ncapabilities:\n  mfa: true\n  dpop: true\n  backchannel_logout: true\n  dynamic_client_registration: true\n  global_token_revocation: true\n  pkce: true\ngaps:\n- 'No public API reference documents how to obtain credentials, what audience to request, or which scopes gate which operation.'\n- 'No API-key or mutualTLS scheme is advertised anywhere public.'\n- 'The password and implicit grants remain enabled on the tenant; both are discouraged by OAuth 2.1.'\nx-evidence:\n  fetched: '2026-08-26'\n  url: https://auth.rapiddeploy.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rapiddeploy/refs/heads/main/authentication/rapiddeploy-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Public Safety
- Emergency Services
- NG911
- Computer-Aided Dispatch
- Mapping
- Analytics
- Government
- Cloud
---
