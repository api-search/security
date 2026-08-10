---
api_key_in: []
auth_types: []
description: OncoC4 publishes no developer-facing API and therefore no developer authentication scheme. The only authentication surface reachable anonymously on oncoc4.com is the Umbraco CMS Delivery API *member* authorization server, whose OpenID Connect discovery document is served at /.well-known/openid-configuration. This profile is derived verbatim from that document. It describes website member login, not an API product.
kind: authentication
layout: security
method: probed
name: Oncoc4 Authentication
name_suffix: Authentication
oauth_flows: []
overview: OncoC4 declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: OncoC4
provider_slug: oncoc4
scheme_count: 1
schemes:
- claims:
  - aud
  - exp
  - iat
  - iss
  - sub
  endpoints:
    authorization: https://oncoc4.com/umbraco/delivery/api/v1/security/member/authorize
    end_session: https://oncoc4.com/umbraco/delivery/api/v1/security/member/signout
    jwks: https://oncoc4.com/.well-known/jwks
    revocation: https://oncoc4.com/umbraco/delivery/api/v1/security/member/revoke
    token: https://oncoc4.com/umbraco/delivery/api/v1/security/member/token
    userinfo: https://oncoc4.com/umbraco/delivery/api/v1/security/member/userinfo
  features:
    authorization_response_iss_parameter_supported: true
    claims_parameter_supported: false
    request_parameter_supported: false
    request_uri_parameter_supported: false
  grant_types:
  - authorization_code
  - refresh_token
  id: umbraco_delivery_member_oidc
  id_token_signing_alg_values:
  - RS256
  issuer: https://oncoc4.com/
  openIdConnectUrl: https://oncoc4.com/.well-known/openid-configuration
  pkce:
    code_challenge_methods:
    - plain
    - S256
    supported: true
  response_modes:
  - form_post
  - fragment
  - query
  response_types:
  - code
  scopes:
  - openid
  - offline_access
  standard: OpenID Connect 1.0 / OAuth 2.0
  subject_types:
  - public
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
slug: oncoc4-authentication
source_filename: oncoc4-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://oncoc4.com/.well-known/openid-configuration\nname: OncoC4 authentication profile\ndescription: >-\n  OncoC4 publishes no developer-facing API and therefore no developer\n  authentication scheme. The only authentication surface reachable anonymously on\n  oncoc4.com is the Umbraco CMS Delivery API *member* authorization server, whose\n  OpenID Connect discovery document is served at /.well-known/openid-configuration.\n  This profile is derived verbatim from that document. It describes website member\n  login, not an API product.\ncaveat: >-\n  Not a developer API auth profile. Umbraco ships this authorization server by\n  default with the Delivery API; its presence says nothing about an API program.\n  The endpoints it advertises live under /umbraco/, which oncoc4.com/robots.txt\n  disallows, so they were not crawled.\nschemes:\n- id: umbraco_delivery_member_oidc\n  type: openIdConnect\n  standard: OpenID Connect 1.0 /\
  \ OAuth 2.0\n  openIdConnectUrl: https://oncoc4.com/.well-known/openid-configuration\n  issuer: https://oncoc4.com/\n  endpoints:\n    authorization: https://oncoc4.com/umbraco/delivery/api/v1/security/member/authorize\n    token: https://oncoc4.com/umbraco/delivery/api/v1/security/member/token\n    userinfo: https://oncoc4.com/umbraco/delivery/api/v1/security/member/userinfo\n    end_session: https://oncoc4.com/umbraco/delivery/api/v1/security/member/signout\n    revocation: https://oncoc4.com/umbraco/delivery/api/v1/security/member/revoke\n    jwks: https://oncoc4.com/.well-known/jwks\n  grant_types:\n  - authorization_code\n  - refresh_token\n  response_types:\n  - code\n  response_modes:\n  - form_post\n  - fragment\n  - query\n  pkce:\n    supported: true\n    code_challenge_methods:\n    - plain\n    - S256\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  id_token_signing_alg_values:\n  - RS256\n  subject_types:\n  - public\n  claims:\n  - aud\n\
  \  - exp\n  - iat\n  - iss\n  - sub\n  scopes:\n  - openid\n  - offline_access\n  features:\n    claims_parameter_supported: false\n    request_parameter_supported: false\n    request_uri_parameter_supported: false\n    authorization_response_iss_parameter_supported: true\nnotes:\n- No API key, HTTP bearer, basic, or mutualTLS scheme is documented anywhere on\n  the public OncoC4 surface.\n- PKCE advertises `plain` alongside `S256`; `plain` is a downgrade path and is\n  discouraged by RFC 7636 for public clients.\nx-evidence:\n  fetched: '2026-08-04'\n  url: https://oncoc4.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json;charset=UTF-8\n  file: well-known/oncoc4-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oncoc4/refs/heads/main/authentication/oncoc4-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Biotechnology
- Biopharmaceutical
- Life Sciences
- Oncology
- Immunotherapy
- Clinical Trials
- Healthcare
- Pharmaceuticals
---
