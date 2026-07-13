---
api_key_in: []
api_specs:
- filename: openapi.yml
  format: yaml
  label: Authelia REST API
  slug: authelia-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/authelia/authelia/master/api/openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Authelia Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Authelia secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Authelia
provider_slug: authelia
scheme_count: 3
schemes:
- description: RFC 6749 client_secret_basic for token, introspection and revocation endpoints.
  name: clientBasicAuth
  scheme: basic
  sources:
  - openapi/authelia-openapi.yml
  type: http
- description: Bearer access token for UserInfo and other protected endpoints.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/authelia-openapi.yml
  type: http
- flows:
  - authorizationUrl: https://auth.example.com/api/oidc/authorization
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://auth.example.com/api/oidc/token
  name: oauth2
  sources:
  - openapi/authelia-openapi.yml
  type: oauth2
slug: authelia-authentication
source_filename: authelia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/authelia-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: clientBasicAuth\n  type: http\n  scheme: basic\n  description: RFC 6749 client_secret_basic for token, introspection and revocation endpoints.\n  sources:\n  - openapi/authelia-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer access token for UserInfo and other protected endpoints.\n  sources:\n  - openapi/authelia-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.example.com/api/oidc/authorization\n    tokenUrl: https://auth.example.com/api/oidc/token\n    scopes: 5\n  sources:\n  - openapi/authelia-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/authentication/authelia-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Authentication
- Authorization
- LDAP
- MFA
- Open Source
- OpenID Connect
- Self-Hosted
- SSO
---
