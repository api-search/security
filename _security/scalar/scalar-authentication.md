---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Scalar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scalar secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Scalar
provider_slug: scalar
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/scalar-core.json
  type: http
slug: scalar-authentication
source_filename: scalar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/scalar-core.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/scalar-core.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scalar/refs/heads/main/authentication/scalar-authentication.yml
summary_line: http · 1 scheme
tags:
- API Client
- API Documentation
- API References
- Code Generation
- Developer Tools
- OpenAPI
- Registry
- SDKs
- Swagger
---
