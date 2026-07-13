---
api_key_in: []
api_specs:
- filename: northflank-openapi.yml
  format: yaml
  label: Northflank API
  slug: northflank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/northflank/refs/heads/main/openapi/northflank-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Northflank Authentication
name_suffix: Authentication
oauth_flows: []
overview: Northflank secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Northflank
provider_slug: northflank
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/northflank-openapi.yml
  type: http
slug: northflank-authentication
source_filename: northflank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/northflank-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/northflank-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/northflank/refs/heads/main/authentication/northflank-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud Deployment
- Developer Experience
- Internal Developer Platform
- Platform Engineering
---
