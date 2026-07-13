---
api_key_in:
- header
api_specs:
- filename: reflect-openapi.yml
  format: yaml
  label: Reflect
  slug: reflect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reflect/refs/heads/main/openapi/reflect-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Reflect Authentication
name_suffix: Authentication
oauth_flows: []
overview: Reflect secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Reflect
provider_slug: reflect
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/reflect-openapi.yml
  type: apiKey
slug: reflect-authentication
source_filename: reflect-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/reflect-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/reflect-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reflect/refs/heads/main/authentication/reflect-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI Testing
- Artificial Intelligence
- Automated Testing
- CI/CD
- End-to-End Testing
- QA
- Testing
---
