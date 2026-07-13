---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gluu Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gluu secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gluu
provider_slug: gluu
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 access token with SCIM scopes
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/gluu-openapi.yml
  type: http
slug: gluu-authentication
source_filename: gluu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gluu-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 access token with SCIM scopes\n  sources:\n  - openapi/gluu-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gluu/refs/heads/main/authentication/gluu-authentication.yml
summary_line: http · 1 scheme
tags:
- Access Management
- Authentication
- Authorization
- IAM
- Identities
- OAuth
- OpenID Connect
---
