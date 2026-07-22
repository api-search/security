---
api_key_in:
- header
api_specs:
- filename: skilljar-openapi-original.yml
  format: yaml
  label: Skilljar API
  slug: skilljar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skilljar/refs/heads/main/openapi/skilljar-openapi-original.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Skilljar Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Skilljar secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Skilljar
provider_slug: skilljar
scheme_count: 3
schemes:
- description: API key authentication using HTTP Basic Auth. Use your API key as the username and leave the password empty.
  in: header
  name: OrganizationApiKey
  scheme: basic
  sources:
  - openapi/skilljar-openapi-original.yml
  type: http
- description: Bearer token authentication.
  name: tokenAuth
  scheme: bearer
  sources:
  - openapi/skilljar-openapi-original.yml
  type: http
- flows:
  - authorizationUrl: https://dashboard.skilljar.com/oauth/authorize
    flow: authorizationCode
    pkce: S256
    refreshUrl: https://api.skilljar.com/v2/auth/token
    scope_count: 89
    tokenUrl: https://api.skilljar.com/v2/auth/token
  jwks_uri: https://api.skilljar.com/.well-known/jwks.json
  name: OAuth2
  registration_endpoint: https://api.skilljar.com/v2/oauth/register
  revocation_endpoint: https://api.skilljar.com/v2/auth/revoke
  sources:
  - https://api.skilljar.com/.well-known/oauth-authorization-server
  type: oauth2
slug: skilljar-authentication
source_filename: skilljar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/skilljar-openapi-original.yml\ndocs: https://support.gainsight.com/Skilljar/Develop_and_Customize/API/Getting_started_with_the_Skilljar_API\nsummary:\n  types:\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  note: >-\n    Skilljar exposes two authentication surfaces. The v1 REST API authenticates\n    with an Organization API key sent via HTTP Basic (API key as the username,\n    empty password). A newer v2 OAuth 2.0 surface (advertised via RFC 8414\n    Authorization Server Metadata at /.well-known/oauth-authorization-server)\n    supports authorization_code + refresh_token with PKCE (S256), dynamic client\n    registration, and ~89 granular scopes.\nschemes:\n- name: OrganizationApiKey\n  type: http\n  scheme: basic\n  in: header\n  description: >-\n    API key authentication using HTTP Basic Auth. Use your API key as the\n    username and leave the password empty.\n  sources:\n\
  \  - openapi/skilljar-openapi-original.yml\n- name: tokenAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication.\n  sources:\n  - openapi/skilljar-openapi-original.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://dashboard.skilljar.com/oauth/authorize\n    tokenUrl: https://api.skilljar.com/v2/auth/token\n    refreshUrl: https://api.skilljar.com/v2/auth/token\n    pkce: S256\n    scope_count: 89\n  registration_endpoint: https://api.skilljar.com/v2/oauth/register\n  revocation_endpoint: https://api.skilljar.com/v2/auth/revoke\n  jwks_uri: https://api.skilljar.com/.well-known/jwks.json\n  sources:\n  - https://api.skilljar.com/.well-known/oauth-authorization-server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skilljar/refs/heads/main/authentication/skilljar-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Education
- Learning Management System
- Customer Education
- Training
- Online Courses
- Certification
- Webhooks
- Enrollment
---
