---
api_key_in: []
api_specs:
- filename: calm-partner-api-openapi.yml
  format: yaml
  label: Calm Partner API
  slug: calm-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calm-com/refs/heads/main/openapi/calm-partner-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Calm Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Calm secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Calm
provider_slug: calm-com
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT access token issued by POST /v0/authorize.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/calm-partner-api-openapi.yml
  type: http
slug: calm-com-authentication
source_filename: calm-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/calm-partner-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT access token issued by POST /v0/authorize.\n  sources:\n  - openapi/calm-partner-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/calm-com/refs/heads/main/authentication/calm-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Mindfulness
- Meditation
- Sleep
- Mental Health
- Wellness
- Digital Health
- Mobile App
- Consumer
- Employee Wellness
- Digital Therapeutics
- B2B
---
