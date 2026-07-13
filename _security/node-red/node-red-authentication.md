---
api_key_in: []
api_specs:
- filename: node-red-admin-openapi.yml
  format: yaml
  label: Node-RED Admin API
  slug: node-red
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/node-red/refs/heads/main/openapi/node-red-admin-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Node Red Authentication
name_suffix: Authentication
oauth_flows: []
overview: Node-RED secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Node-RED
provider_slug: node-red
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/node-red-admin-openapi.yml
  type: http
slug: node-red-authentication
source_filename: node-red-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/node-red-admin-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/node-red-admin-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/node-red/refs/heads/main/authentication/node-red-authentication.yml
summary_line: http · 1 scheme
tags:
- Self-Hosted
- Workflow Automation
- Flow-Based Programming
- IoT
---
