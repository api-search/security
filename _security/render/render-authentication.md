---
api_key_in: []
api_specs:
- filename: render-openapi.json
  format: json
  label: Render API
  slug: render-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/render/refs/heads/main/openapi/render-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Render Authentication
name_suffix: Authentication
oauth_flows: []
overview: Render secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Render
provider_slug: render
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/render-openapi.json
  type: http
slug: render-authentication
source_filename: render-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/render-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/render-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/render/refs/heads/main/authentication/render-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud
- Platform
- Deployment
- Infrastructure
- DevOps
- Web Services
- Databases
- Hosting
---
