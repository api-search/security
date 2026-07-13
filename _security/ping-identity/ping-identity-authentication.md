---
api_key_in: []
api_specs:
- filename: ping-identity-openapi.yaml
  format: yaml
  label: PingOne Platform API
  slug: pingone-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ping-identity/refs/heads/main/openapi/ping-identity-openapi.yaml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Ping Identity Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Ping Identity secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Ping Identity
provider_slug: ping-identity
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ping-identity-openapi.yaml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: /as/token
  - authorizationUrl: /as/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: /as/token
  name: oauth2
  sources:
  - openapi/ping-identity-openapi.yaml
  type: oauth2
slug: ping-identity-authentication
source_filename: ping-identity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ping-identity-openapi.yaml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/ping-identity-openapi.yaml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /as/token\n    scopes: 0\n  - flow: authorizationCode\n    authorizationUrl: /as/authorize\n    tokenUrl: /as/token\n    scopes: 0\n  sources:\n  - openapi/ping-identity-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ping-identity/refs/heads/main/authentication/ping-identity-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Identity
- Authentication
- Authorization
- SSO
- MFA
---
