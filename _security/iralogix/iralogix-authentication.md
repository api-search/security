---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Iralogix Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- implicit
- password
- deviceCode
- tokenExchange
- jwtBearer
overview: IRALOGIX secures its APIs with openIdConnect and oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, implicit, password, deviceCode, tokenExchange, and jwtBearer flow(s).
provider_name: IRALOGIX
provider_slug: iralogix
scheme_count: 1
schemes:
- backchannel_logout_session_supported: true
  backchannel_logout_supported: true
  code_challenge_methods_supported:
  - S256
  - plain
  dpop_supported: true
  endpoints:
    authorization: https://auth.partner.iralogix.com/authorize
    backchannel_authentication: present
    device_authorization: https://auth.partner.iralogix.com/oauth/device/code
    end_session: https://auth.partner.iralogix.com/oidc/logout
    global_token_revocation: present
    jwks: https://auth.partner.iralogix.com/.well-known/jwks.json
    mfa_challenge: https://auth.partner.iralogix.com/mfa/challenge
    registration: https://auth.partner.iralogix.com/oidc/register
    revocation: https://auth.partner.iralogix.com/oauth/revoke
    token: https://auth.partner.iralogix.com/oauth/token
    userinfo: https://auth.partner.iralogix.com/userinfo
  grant_types_supported:
  - client_credentials
  - authorization_code
  - refresh_token
  - password
  - implicit
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - http://auth0.com/oauth/grant-type/password-realm
  - http://auth0.com/oauth/grant-type/passwordless/otp
  - http://auth0.com/oauth/grant-type/mfa-oob
  - http://auth0.com/oauth/grant-type/mfa-otp
  - http://auth0.com/oauth/grant-type/mfa-recovery-code
  id_token_signing_alg_values_supported:
  - HS256
  - RS256
  - PS256
  issuer: https://auth.partner.iralogix.com/
  name: IRALOGIX Partner OIDC
  openIdConnectUrl: https://auth.partner.iralogix.com/.well-known/openid-configuration
  request_parameter_supported: false
  request_uri_parameter_supported: false
  response_modes_supported:
  - query
  - fragment
  - form_post
  response_types_supported:
  - code
  - token
  - id_token
  - code token
  - code id_token
  - token id_token
  - code token id_token
  sources:
  - well-known/iralogix-openid-configuration.json
  subject_types_supported:
  - public
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  token_endpoint_auth_signing_alg_values_supported:
  - RS256
  - RS384
  - PS256
  type: openIdConnect
  vendor: Auth0
slug: iralogix-authentication
source_filename: iralogix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://auth.partner.iralogix.com/.well-known/openid-configuration\ndocs: null\nnotes: 'Derived entirely from the live OIDC discovery document IRALOGIX publishes for\n  its partner platform. There is no public OpenAPI to derive securitySchemes from —\n  the partner documentation (docs.iralogix.com) is behind Okta visitor authentication\n  and the partner console (partner.iralogix.com) behind this Auth0 tenant. A second,\n  separate Okta org (iralogix.okta.com) fronts the documentation site itself.'\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\n  - password\n  - deviceCode\n  - tokenExchange\n  - jwtBearer\n  api_key_in: []\n  pkce: true\n  mfa: true\n  dynamic_client_registration: true\nschemes:\n- name: IRALOGIX Partner OIDC\n  type: openIdConnect\n  openIdConnectUrl: https://auth.partner.iralogix.com/.well-known/openid-configuration\n  issuer:\
  \ https://auth.partner.iralogix.com/\n  vendor: Auth0\n  sources:\n  - well-known/iralogix-openid-configuration.json\n  endpoints:\n    authorization: https://auth.partner.iralogix.com/authorize\n    token: https://auth.partner.iralogix.com/oauth/token\n    device_authorization: https://auth.partner.iralogix.com/oauth/device/code\n    userinfo: https://auth.partner.iralogix.com/userinfo\n    mfa_challenge: https://auth.partner.iralogix.com/mfa/challenge\n    jwks: https://auth.partner.iralogix.com/.well-known/jwks.json\n    registration: https://auth.partner.iralogix.com/oidc/register\n    revocation: https://auth.partner.iralogix.com/oauth/revoke\n    end_session: https://auth.partner.iralogix.com/oidc/logout\n    backchannel_authentication: present\n    global_token_revocation: present\n  grant_types_supported:\n  - client_credentials\n  - authorization_code\n  - refresh_token\n  - password\n  - implicit\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n\
  \  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - http://auth0.com/oauth/grant-type/password-realm\n  - http://auth0.com/oauth/grant-type/passwordless/otp\n  - http://auth0.com/oauth/grant-type/mfa-oob\n  - http://auth0.com/oauth/grant-type/mfa-otp\n  - http://auth0.com/oauth/grant-type/mfa-recovery-code\n  response_types_supported:\n  - code\n  - token\n  - id_token\n  - code token\n  - code id_token\n  - token id_token\n  - code token id_token\n  response_modes_supported:\n  - query\n  - fragment\n  - form_post\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\n  token_endpoint_auth_signing_alg_values_supported:\n  - RS256\n  - RS384\n  - PS256\n  id_token_signing_alg_values_supported:\n  - HS256\n  - RS256\n  - PS256\n  code_challenge_methods_supported:\n  - S256\n  - plain\n  subject_types_supported:\n  - public\n  backchannel_logout_supported: true\n  backchannel_logout_session_supported: true\n  request_parameter_supported:\
  \ false\n  request_uri_parameter_supported: false\n  dpop_supported: true\nobservations:\n- id: pkce-s256\n  note: PKCE S256 is advertised; `plain` is also still advertised, which RFC 7636 §4.2\n    discourages for clients able to do S256.\n- id: implicit-and-password-grants\n  note: The implicit and resource-owner-password grants remain enabled on the tenant.\n    OAuth 2.1 and the Auth0 defaults both deprecate these; a partner-facing financial\n    platform would normally disable both.\n- id: private-key-jwt\n  note: private_key_jwt client authentication is supported, which is the FAPI-preferred\n    method for confidential clients.\n- id: no-par\n  note: No pushed_authorization_request_endpoint and no request_object_signing_alg_values_supported\n    — PAR and signed request objects are not advertised, so the tenant is not FAPI 2.0\n    profile-ready as configured.\nx-evidence:\n  fetched: '2026-08-04'\n  url: https://auth.partner.iralogix.com/.well-known/openid-configuration\n  http_status:\
  \ 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iralogix/refs/heads/main/authentication/iralogix-authentication.yml
summary_line: openIdConnect/oauth2 · 1 scheme
tags:
- Company
- Financial Services
- Retirement
- IRA
- Recordkeeping
- Wealth Management
- Fintech
- Compliance
- White Label
- Retirement Technology
---
