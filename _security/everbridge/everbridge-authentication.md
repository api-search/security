---
api_key_in: []
api_specs:
- filename: swagger.json
  format: json
  label: Everbridge Suite API
  slug: everbridge-suite-api
  spec_type: OpenAPI
  url: https://api.everbridge.net/rest/swagger.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Everbridge Authentication
name_suffix: Authentication
oauth_flows: []
overview: Everbridge secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Everbridge
provider_slug: everbridge
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 id_token from /authorization/v1/tokens
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/everbridge-openapi.yml
  type: http
slug: everbridge-authentication
source_filename: everbridge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/everbridge-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 id_token from /authorization/v1/tokens\n  sources:\n  - openapi/everbridge-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/everbridge/refs/heads/main/authentication/everbridge-authentication.yml
summary_line: http · 1 scheme
tags:
- Critical Event Management
- Emergency Management
- Incident Management
- IT Alerting
- Mass Notification
---
