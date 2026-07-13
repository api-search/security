---
api_key_in: []
api_specs:
- filename: retool-management-api-openapi.yml
  format: yaml
  label: Retool Management API
  slug: retool-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/retool/refs/heads/main/openapi/retool-management-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Retool Authentication
name_suffix: Authentication
oauth_flows: []
overview: Retool secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Retool
provider_slug: retool
scheme_count: 1
schemes:
- description: 'Bearer token generated in Retool workspace settings under API Access Tokens. Format: Authorization: Bearer <token>'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/retool-management-api-openapi.yml
  type: http
slug: retool-authentication
source_filename: retool-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/retool-management-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Bearer token generated in Retool workspace settings under API Access Tokens.\n    Format: Authorization: Bearer <token>'\n  sources:\n  - openapi/retool-management-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/retool/refs/heads/main/authentication/retool-authentication.yml
summary_line: http · 1 scheme
tags:
- Admin Panel
- Dashboard
- Internal Tools
- Low Code
- No Code
---
