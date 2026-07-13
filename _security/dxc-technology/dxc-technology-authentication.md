---
api_key_in: []
api_specs:
- filename: dxc-developer-central-api-openapi.yml
  format: yaml
  label: DXC Developer Central API
  slug: developer-central-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dxc-technology/refs/heads/main/openapi/dxc-developer-central-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dxc Technology Authentication
name_suffix: Authentication
oauth_flows: []
overview: DXC Technology secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DXC Technology
provider_slug: dxc-technology
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/dxc-developer-central-api-openapi.yml
  type: http
slug: dxc-technology-authentication
source_filename: dxc-technology-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dxc-developer-central-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/dxc-developer-central-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dxc-technology/refs/heads/main/authentication/dxc-technology-authentication.yml
summary_line: http · 1 scheme
tags:
- IT Services
- Enterprise
- Platform
- Integration
---
