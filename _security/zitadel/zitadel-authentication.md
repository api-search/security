---
api_key_in: []
api_specs:
- filename: zitadel-management-openapi.yml
  format: yaml
  label: Zitadel Management API
  slug: management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zitadel/refs/heads/main/openapi/zitadel-management-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Zitadel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zitadel secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zitadel
provider_slug: zitadel
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/zitadel-management-openapi.yml
  type: http
slug: zitadel-authentication
source_filename: zitadel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zitadel-management-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/zitadel-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zitadel/refs/heads/main/authentication/zitadel-authentication.yml
summary_line: http · 1 scheme
tags:
- Authentication
- Authorization
- Identity Management
- Open Source
- OAuth 2.0
- OIDC
---
