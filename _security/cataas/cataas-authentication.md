---
api_key_in: []
api_specs:
- filename: cataas-openapi-original.yml
  format: yaml
  label: Cataas
  slug: cataas
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cataas/refs/heads/main/openapi/cataas-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cataas Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cataas secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cataas
provider_slug: cataas
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Admin-only bearer token for moderation and catalog management.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cataas-openapi-original.yml
  type: http
slug: cataas-authentication
source_filename: cataas-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cataas-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Admin-only bearer token for moderation and catalog management.\n  sources:\n  - openapi/cataas-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cataas/refs/heads/main/authentication/cataas-authentication.yml
summary_line: http · 1 scheme
tags:
- Animals
- Cats
- Images
- Open Source
- Public APIs
---
