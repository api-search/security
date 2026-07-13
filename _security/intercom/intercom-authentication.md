---
api_key_in: []
api_specs:
- filename: intercom-openapi.yml
  format: yaml
  label: Intercom API
  slug: intercom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intercom/refs/heads/main/openapi/intercom-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Intercom Authentication
name_suffix: Authentication
oauth_flows: []
overview: Intercom secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Intercom
provider_slug: intercom
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/intercom-openapi.yml
  type: http
slug: intercom-authentication
source_filename: intercom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/intercom-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/intercom-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intercom/refs/heads/main/authentication/intercom-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Customer Service
- Customer Support
- Messaging
---
