---
api_key_in:
- header
api_specs:
- filename: superblocks-applications-api-openapi.yml
  format: yaml
  label: Superblocks Applications API
  slug: superblocks-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superblocks/refs/heads/main/openapi/superblocks-applications-api-openapi.yml
- filename: superblocks-workflows-api-openapi.yml
  format: yaml
  label: Superblocks Workflows API
  slug: superblocks-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/superblocks/refs/heads/main/openapi/superblocks-workflows-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Superblocks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Superblocks secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Superblocks
provider_slug: superblocks
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/superblocks-superblocks-api-openapi.yml
  type: http
- in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/superblocks-superblocks-api-openapi.yml
  type: apiKey
slug: superblocks-authentication
source_filename: superblocks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/superblocks-superblocks-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/superblocks-superblocks-api-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/superblocks-superblocks-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superblocks/refs/heads/main/authentication/superblocks-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Internal Tools
- Low-Code
- No-Code
- Application
- Workflows
- Scheduled Jobs
- Integration
- Enterprise
- Artificial Intelligence
- Databases
- REST API
- Developer Tools
---
