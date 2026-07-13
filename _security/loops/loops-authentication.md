---
api_key_in: []
api_specs:
- filename: loops-openapi.yaml
  format: yaml
  label: Loops API
  slug: loops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Loops Authentication
name_suffix: Authentication
oauth_flows: []
overview: Loops secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Loops
provider_slug: loops
scheme_count: 1
schemes:
- name: apiKey
  scheme: bearer
  sources:
  - openapi/loops-openapi.yaml
  type: http
slug: loops-authentication
source_filename: loops-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/loops-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/loops-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/authentication/loops-authentication.yml
summary_line: http · 1 scheme
tags:
- Email
- Marketing Automation
- Transactional Email
- SaaS
- Communications
---
