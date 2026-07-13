---
api_key_in: []
api_specs:
- filename: caspio-openapi.yml
  format: yaml
  label: Caspio REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caspio/refs/heads/main/openapi/caspio-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Caspio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Caspio secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Caspio
provider_slug: caspio
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/caspio-openapi.yml
  type: http
slug: caspio-authentication
source_filename: caspio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/caspio-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/caspio-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caspio/refs/heads/main/authentication/caspio-authentication.yml
summary_line: http · 1 scheme
tags:
- Low Code
- No Code
- Database
- Application Platform
- Cloud Database
- Online Forms
- Workflow Automation
---
