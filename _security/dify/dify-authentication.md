---
api_key_in: []
api_specs:
- filename: dify-openapi.yml
  format: yaml
  label: Dify
  slug: dify
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/openapi/dify-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dify secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dify
provider_slug: dify
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/dify-openapi.yml
  type: http
slug: dify-authentication
source_filename: dify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dify-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/dify-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dify/refs/heads/main/authentication/dify-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Backend-As-A-Service
- LLMOps
---
