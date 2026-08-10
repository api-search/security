---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Employeenavigator Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
- implicit
- deviceCode
- ciba
overview: Employee Navigator secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, refreshToken, implicit, deviceCode, and ciba flow(s).
provider_name: Employee Navigator
provider_slug: employeenavigator
scheme_count: 2
schemes:
- issuer: https://www.employeenavigator.com/identity
  name: OpenIDConnect
  openIdConnectUrl: https://www.employeenavigator.com/identity/.well-known/openid-configuration
  sources:
  - well-known/employeenavigator-openid-configuration.json
  type: openIdConnect
- flows:
  - authorizationUrl: https://www.employeenavigator.com/identity/connect/authorize
    flow: authorizationCode
    refreshUrl: https://www.employeenavigator.com/identity/connect/token
    tokenUrl: https://www.employeenavigator.com/identity/connect/token
  - flow: clientCredentials
    tokenUrl: https://www.employeenavigator.com/identity/connect/token
  - authorizationUrl: https://www.employeenavigator.com/identity/connect/authorize
    flow: implicit
  - deviceAuthorizationUrl: https://www.employeenavigator.com/identity/connect/deviceauthorization
    flow: deviceCode
    grant_type: urn:ietf:params:oauth:grant-type:device_code
    tokenUrl: https://www.employeenavigator.com/identity/connect/token
  - backchannelAuthenticationUrl: https://www.employeenavigator.com/identity/connect/ciba
    delivery_modes:
    - poll
    flow: ciba
    grant_type: urn:openid:params:grant-type:ciba
  name: OAuth2
  sources:
  - well-known/employeenavigator-openid-configuration.json
  type: oauth2
slug: employeenavigator-authentication
source_filename: employeenavigator-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: https://www.employeenavigator.com/identity/.well-known/openid-configuration\ndocs: https://www.employeenavigator.com/security/\nnotes: >-\n  Derived verbatim from the anonymously-served OpenID Connect discovery document\n  at the Employee Navigator identity host, not from an OpenAPI securitySchemes\n  block — Employee Navigator publishes no public OpenAPI. The server is a Duende\n  IdentityServer instance mounted at /identity on the apex web host and fronts\n  every named Employee Navigator platform API service (see\n  scopes/employeenavigator-scopes.yml).\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - refreshToken\n  - implicit\n  - deviceCode\n  - ciba\n  bearer_format: JWT\n  scope_count: 66\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://www.employeenavigator.com/identity/.well-known/openid-configuration\n\
  \  issuer: https://www.employeenavigator.com/identity\n  sources:\n  - well-known/employeenavigator-openid-configuration.json\n- name: OAuth2\n  type: oauth2\n  sources:\n  - well-known/employeenavigator-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.employeenavigator.com/identity/connect/authorize\n    tokenUrl: https://www.employeenavigator.com/identity/connect/token\n    refreshUrl: https://www.employeenavigator.com/identity/connect/token\n  - flow: clientCredentials\n    tokenUrl: https://www.employeenavigator.com/identity/connect/token\n  - flow: implicit\n    authorizationUrl: https://www.employeenavigator.com/identity/connect/authorize\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://www.employeenavigator.com/identity/connect/deviceauthorization\n    tokenUrl: https://www.employeenavigator.com/identity/connect/token\n    grant_type: urn:ietf:params:oauth:grant-type:device_code\n  - flow: ciba\n    backchannelAuthenticationUrl:\
  \ https://www.employeenavigator.com/identity/connect/ciba\n    grant_type: urn:openid:params:grant-type:ciba\n    delivery_modes:\n    - poll\nendpoints:\n  issuer: https://www.employeenavigator.com/identity\n  authorization: https://www.employeenavigator.com/identity/connect/authorize\n  token: https://www.employeenavigator.com/identity/connect/token\n  userinfo: https://www.employeenavigator.com/identity/connect/userinfo\n  jwks: https://www.employeenavigator.com/identity/.well-known/openid-configuration/jwks\n  introspection: https://www.employeenavigator.com/identity/connect/introspect\n  revocation: https://www.employeenavigator.com/identity/connect/revocation\n  end_session: https://www.employeenavigator.com/identity/connect/endsession\n  check_session_iframe: https://www.employeenavigator.com/identity/connect/checksession\n  device_authorization: https://www.employeenavigator.com/identity/connect/deviceauthorization\n  backchannel_authentication: https://www.employeenavigator.com/identity/connect/ciba\n\
  client_authentication:\n- client_secret_basic\n- client_secret_post\nproof_of_possession:\n  pkce: true\n  pkce_methods:\n  - plain\n  - S256\n  dpop: true\n  dpop_signing_algs:\n  - RS256\n  - RS384\n  - RS512\n  - PS256\n  - PS384\n  - PS512\n  - ES256\n  - ES384\n  - ES512\ntokens:\n  id_token_signing_algs:\n  - RS256\n  subject_types:\n  - public\n  offline_access: true\n  request_object_supported: true\nlogout:\n  frontchannel_logout: true\n  frontchannel_logout_session: true\n  backchannel_logout: true\n  backchannel_logout_session: true\nclaims:\n- sub\n- name\n- family_name\n- given_name\n- middle_name\n- nickname\n- preferred_username\n- profile\n- picture\n- website\n- gender\n- birthdate\n- zoneinfo\n- locale\n- updated_at\n- email\n- email_verified\nprompt_values:\n- none\n- login\n- consent\n- select_account\nresponse_types:\n- code\n- token\n- id_token\n- id_token token\n- code id_token\n- code token\n- code id_token token\nresponse_modes:\n- form_post\n- query\n- fragment\n\
  x-evidence:\n  fetched: '2026-08-06'\n  url: https://www.employeenavigator.com/identity/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json; charset=UTF-8\nx-access:\n  client_registration: manual\n  note: >-\n    No dynamic client registration endpoint is advertised. API client\n    credentials are issued to carriers, payroll companies and other partners\n    through Employee Navigator's partner onboarding; there is no public\n    self-service developer signup.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/employeenavigator/refs/heads/main/authentication/employeenavigator-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Benefits Administration
- Human Resources
- Insurance
- Employee Benefits
- Payroll
- Health Insurance
- HRIS
- Open Enrollment
- ACA Compliance
- Identity
- OpenID Connect
---
