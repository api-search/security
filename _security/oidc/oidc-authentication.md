---
api_key_in: []
api_specs:
- filename: oidc-authentication-api-openapi.yml
  format: yaml
  label: OIDC Authentication API
  slug: oidc-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oidc/refs/heads/main/openapi/oidc-authentication-api-openapi.yml
- filename: oidc-discovery-api-openapi.yml
  format: yaml
  label: OIDC Discovery API
  slug: oidc-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oidc/refs/heads/main/openapi/oidc-discovery-api-openapi.yml
- filename: oidc-jwks-api-openapi.yml
  format: yaml
  label: OIDC JWKS API
  slug: oidc-jwks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oidc/refs/heads/main/openapi/oidc-jwks-api-openapi.yml
- filename: oidc-session-api-openapi.yml
  format: yaml
  label: OIDC Session API
  slug: oidc-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oidc/refs/heads/main/openapi/oidc-session-api-openapi.yml
- filename: oidc-token-api-openapi.yml
  format: yaml
  label: OIDC Token API
  slug: oidc-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oidc/refs/heads/main/openapi/oidc-token-api-openapi.yml
- filename: oidc-userinfo-api-openapi.yml
  format: yaml
  label: OIDC UserInfo API
  slug: oidc-userinfo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oidc/refs/heads/main/openapi/oidc-userinfo-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Oidc Authentication
name_suffix: Authentication
oauth_flows: []
overview: OIDC secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OIDC
provider_slug: oidc
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 Bearer Token obtained through OIDC authentication.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/oidc.yml
  type: http
slug: oidc-authentication
source_filename: oidc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/oidc.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 Bearer Token obtained through OIDC authentication.\n  sources:\n  - openapi/oidc.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oidc/refs/heads/main/authentication/oidc-authentication.yml
summary_line: http · 1 scheme
tags:
- Authentication
- Identity
- JWT
- OIDC
- OpenID Connect
---
