---
api_key_in: []
api_specs:
- filename: rippling-webhooks-asyncapi.yml
  format: yaml
  label: Rippling Webhooks API
  slug: rippling-webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/rippling/refs/heads/main/asyncapi/rippling-webhooks-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Rippling Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rippling secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rippling
provider_slug: rippling
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Rippling API tokens are issued via OAuth2 (or generated as personal/app

    tokens) and supplied as `Authorization: Bearer <token>`.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/rippling-openapi.yml
  type: http
slug: rippling-authentication
source_filename: rippling-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rippling-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    Rippling API tokens are issued via OAuth2 (or generated as personal/app\n    tokens) and supplied as `Authorization: Bearer <token>`.\n  sources:\n  - openapi/rippling-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rippling/refs/heads/main/authentication/rippling-authentication.yml
summary_line: http · 1 scheme
tags:
- HR
- HCM
- Payroll
- IT
- Identity
- SCIM
- Devices
- Spend Management
---
