---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Concertai Authentication
name_suffix: Authentication
oauth_flows:
- authorization_code
- client_credentials
- refresh_token
- device_code
- implicit
- password
- token_exchange
- jwt_bearer
overview: ConcertAI secures its APIs with openIdConnect and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorization_code, client_credentials, refresh_token, device_code, implicit, password, token_exchange, and jwt_bearer flow(s).
provider_name: ConcertAI
provider_slug: concertai
scheme_count: 2
schemes:
- authorization_endpoint: https://auth.precision.concertai.com/authorize
  backchannel_authentication_endpoint: https://auth.precision.concertai.com/bc-authorize
  backchannel_logout_supported: true
  device_authorization_endpoint: https://auth.precision.concertai.com/oauth/device/code
  end_session_endpoint: https://auth.precision.concertai.com/oidc/logout
  id_token_signing_alg_values_supported:
  - HS256
  - RS256
  - PS256
  issuer: https://auth.precision.concertai.com/
  jwks_uri: https://auth.precision.concertai.com/.well-known/jwks.json
  name: precision-oidc
  openIdConnectUrl: https://auth.precision.concertai.com/.well-known/openid-configuration
  registration_endpoint: https://auth.precision.concertai.com/oidc/register
  revocation_endpoint: https://auth.precision.concertai.com/oauth/revoke
  sources:
  - well-known/concertai-precision-openid-configuration.json
  subject_types_supported:
  - public
  token_endpoint: https://auth.precision.concertai.com/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
  userinfo_endpoint: https://auth.precision.concertai.com/userinfo
- issuer: https://login.precision.concertai.com/
  name: precision-login-oidc
  note: second Auth0 custom domain with an identical metadata document
  openIdConnectUrl: https://login.precision.concertai.com/.well-known/openid-configuration
  sources:
  - well-known/concertai-precision-login-openid-configuration.json
  type: openIdConnect
slug: concertai-authentication
source_filename: concertai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: https://auth.precision.concertai.com/.well-known/openid-configuration\nnote: >-\n  Derived from the OpenID Connect discovery documents ConcertAI serves anonymously on\n  the two identity hosts fronting the authenticated Precision platform. ConcertAI\n  publishes no public API reference, so this is the only machine-readable statement of\n  its authentication model that a member of the public can read. No OpenAPI\n  securitySchemes exist in this repo to derive from.\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - device_code\n  - implicit\n  - password\n  - token_exchange\n  - jwt_bearer\n  pkce: true\n  pkce_methods:\n  - S256\n  - plain\n  dpop: true\n  dpop_algs:\n  - ES256\n  mfa: true\n  dynamic_client_registration: true\n  identity_provider: Auth0 (custom domain)\nschemes:\n- name: precision-oidc\n  type: openIdConnect\n\
  \  issuer: https://auth.precision.concertai.com/\n  openIdConnectUrl: https://auth.precision.concertai.com/.well-known/openid-configuration\n  authorization_endpoint: https://auth.precision.concertai.com/authorize\n  token_endpoint: https://auth.precision.concertai.com/oauth/token\n  userinfo_endpoint: https://auth.precision.concertai.com/userinfo\n  jwks_uri: https://auth.precision.concertai.com/.well-known/jwks.json\n  revocation_endpoint: https://auth.precision.concertai.com/oauth/revoke\n  registration_endpoint: https://auth.precision.concertai.com/oidc/register\n  device_authorization_endpoint: https://auth.precision.concertai.com/oauth/device/code\n  end_session_endpoint: https://auth.precision.concertai.com/oidc/logout\n  backchannel_authentication_endpoint: https://auth.precision.concertai.com/bc-authorize\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\n  id_token_signing_alg_values_supported:\n  - HS256\n\
  \  - RS256\n  - PS256\n  subject_types_supported:\n  - public\n  backchannel_logout_supported: true\n  sources:\n  - well-known/concertai-precision-openid-configuration.json\n- name: precision-login-oidc\n  type: openIdConnect\n  issuer: https://login.precision.concertai.com/\n  openIdConnectUrl: https://login.precision.concertai.com/.well-known/openid-configuration\n  note: second Auth0 custom domain with an identical metadata document\n  sources:\n  - well-known/concertai-precision-login-openid-configuration.json\npublic_api_authentication:\n  documented: false\n  detail: >-\n    No public developer portal or API reference exists, so there is no published\n    authentication guide for an external integrator. API and data access is arranged\n    through a commercial agreement; the TeraRecon Eureka AI-partner onboarding portal\n    is reached through a \"Become A TeraRecon Partner\" contact form rather than a\n    self-service signup.\nx-evidence:\n- url: https://auth.precision.concertai.com/.well-known/openid-configuration\n\
  \  http_status: 200\n  content_type: application/json\n- url: https://login.precision.concertai.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n- url: https://www.concertai.com/.well-known/openid-configuration\n  http_status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/concertai/refs/heads/main/authentication/concertai-authentication.yml
summary_line: openIdConnect/oauth2 · 2 schemes
tags:
- Company
- Healthcare
- Oncology
- Artificial Intelligence
- Real-World Data
- Clinical Trials
- Life Sciences
- Medical Imaging
- Health Data
---
