---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Hcf Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- refreshToken
- password
- clientCredentials
- deviceCode
- ciba
overview: HCF secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, refreshToken, password, clientCredentials, deviceCode, and ciba flow(s).
provider_name: HCF
provider_slug: hcf
scheme_count: 2
schemes:
- audience: HCF members only
  code_challenge_methods_supported:
  - S256
  dpop_signing_alg_values_supported:
  - RS256
  - RS384
  - RS512
  - ES256
  - ES384
  - ES512
  endpoints:
    authorization: https://id.hcf.com.au/oauth2/v1/authorize
    device_authorization: https://id.hcf.com.au/oauth2/v1/device/authorize
    end_session: https://id.hcf.com.au/oauth2/v1/logout
    introspection: https://id.hcf.com.au/oauth2/v1/introspect
    jwks: https://id.hcf.com.au/oauth2/v1/keys
    pushed_authorization_request: https://id.hcf.com.au/oauth2/v1/par
    registration: https://id.hcf.com.au/oauth2/v1/clients
    revocation: https://id.hcf.com.au/oauth2/v1/revoke
    token: https://id.hcf.com.au/oauth2/v1/token
    userinfo: https://id.hcf.com.au/oauth2/v1/userinfo
  grant_types_supported:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:openid:params:grant-type:ciba
  - urn:okta:params:oauth:grant-type:otp
  - urn:okta:params:oauth:grant-type:oob
  id_token_encryption_alg_values_supported:
  - RSA-OAEP-256
  - RSA-OAEP-384
  - RSA-OAEP-512
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://id.hcf.com.au
  name: HCF member sign-in (Okta OIDC)
  openIdConnectUrl: https://id.hcf.com.au/.well-known/openid-configuration
  request_parameter_supported: true
  response_types_supported:
  - code
  - id_token
  - code id_token
  - code token
  - id_token token
  - code id_token token
  scopes_supported:
  - openid
  - email
  - profile
  - address
  - phone
  - offline_access
  - groups
  source: well-known/hcf-openid-configuration.json
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - none
  type: openIdConnect
- audience: Okta tenant administration
  metadata: https://id.hcf.com.au/.well-known/oauth-authorization-server
  name: Okta org authorization server (tenant management)
  note: Adds client_credentials to the grant list and advertises 83 okta.* org scopes. These are stock Okta org-management scopes describing the identity tenant, NOT an HCF insurance API. See scopes/hcf-scopes.yml.
  source: well-known/hcf-oauth-authorization-server.json
  type: oauth2
slug: hcf-authentication
source_filename: hcf-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://id.hcf.com.au/.well-known/openid-configuration\ndocs: https://www.hcf.com.au/about-us/about-HCF/information-security\nscope_note: >-\n  HCF publishes no developer API and issues no third-party API credentials.\n  Everything captured here describes the Okta-hosted identity tenant at\n  id.hcf.com.au that authenticates MEMBERS into the My Membership app and online\n  member services, plus the separate login-gated ASP.NET provider portals. There\n  is no client registration for third parties, no API key issuance, and no\n  published product scope catalog. This is an identity profile, not an API\n  authentication profile.\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - implicit\n  - refreshToken\n  - password\n  - clientCredentials\n  - deviceCode\n  - ciba\n  third_party_credentials: false\n  self_serve_signup_for_developers: false\nschemes:\n- name: HCF\
  \ member sign-in (Okta OIDC)\n  type: openIdConnect\n  openIdConnectUrl: https://id.hcf.com.au/.well-known/openid-configuration\n  issuer: https://id.hcf.com.au\n  source: well-known/hcf-openid-configuration.json\n  audience: HCF members only\n  endpoints:\n    authorization: https://id.hcf.com.au/oauth2/v1/authorize\n    token: https://id.hcf.com.au/oauth2/v1/token\n    userinfo: https://id.hcf.com.au/oauth2/v1/userinfo\n    jwks: https://id.hcf.com.au/oauth2/v1/keys\n    registration: https://id.hcf.com.au/oauth2/v1/clients\n    introspection: https://id.hcf.com.au/oauth2/v1/introspect\n    revocation: https://id.hcf.com.au/oauth2/v1/revoke\n    end_session: https://id.hcf.com.au/oauth2/v1/logout\n    device_authorization: https://id.hcf.com.au/oauth2/v1/device/authorize\n    pushed_authorization_request: https://id.hcf.com.au/oauth2/v1/par\n  response_types_supported:\n  - code\n  - id_token\n  - code id_token\n  - code token\n  - id_token token\n  - code id_token token\n  grant_types_supported:\n\
  \  - authorization_code\n  - implicit\n  - refresh_token\n  - password\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:openid:params:grant-type:ciba\n  - urn:okta:params:oauth:grant-type:otp\n  - urn:okta:params:oauth:grant-type:oob\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  - client_secret_jwt\n  - private_key_jwt\n  - none\n  code_challenge_methods_supported:\n  - S256\n  id_token_signing_alg_values_supported:\n  - RS256\n  id_token_encryption_alg_values_supported:\n  - RSA-OAEP-256\n  - RSA-OAEP-384\n  - RSA-OAEP-512\n  dpop_signing_alg_values_supported:\n  - RS256\n  - RS384\n  - RS512\n  - ES256\n  - ES384\n  - ES512\n  request_parameter_supported: true\n  scopes_supported:\n  - openid\n  - email\n  - profile\n  - address\n  - phone\n  - offline_access\n  - groups\n- name: Okta org authorization server (tenant management)\n  type: oauth2\n  source: well-known/hcf-oauth-authorization-server.json\n  metadata: https://id.hcf.com.au/.well-known/oauth-authorization-server\n\
  \  audience: Okta tenant administration\n  note: >-\n    Adds client_credentials to the grant list and advertises 83 okta.* org\n    scopes. These are stock Okta org-management scopes describing the identity\n    tenant, NOT an HCF insurance API. See scopes/hcf-scopes.yml.\nmfa:\n  required: true\n  factors:\n  - one-time code by SMS\n  - one-time code by email\n  scope: My Membership app and online member services\n  source: https://www.hcf.com.au/about-us/about-HCF/information-security\n  note: >-\n    HCF states multi-factor authentication is mandatory on member account\n    sign-in; the one-time code is valid for 5 minutes and is re-prompted on\n    every login.\nother_gated_surfaces:\n- name: HCF provider portals\n  url: https://www.hcf.com.au/provider-portals/\n  auth: legacy ASP.NET forms login (frmProvHospLogin.aspx,\n    frmProvMedicalLogin.aspx)\n  audience: recognised hospital, medical, dental and ancillary providers\n  api: false\n  note: >-\n    Login-gated web portals, not\
  \ APIs. No OAuth, no documented machine\n    interface, no credential self-service.\nabsent:\n  api_keys: true\n  developer_client_registration: true\n  partner_oauth_program: true\n  mutual_tls: true\n  documented_scopes_for_business_apis: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hcf/refs/heads/main/authentication/hcf-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Insurance
- Australia
- Health Insurance
- Life Insurance
- Travel Insurance
- Pet Insurance
- Carrier
- Not-for-Profit
- Claims
- Member Services
- Partner Gated
- No Public API
---
