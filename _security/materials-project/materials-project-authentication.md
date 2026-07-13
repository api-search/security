---
api_key_in:
- header
api_specs:
- filename: materials-project-openapi.yml
  format: yaml
  label: Materials Project API
  slug: materials-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/materials-project/refs/heads/main/openapi/materials-project-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Materials Project Authentication
name_suffix: Authentication
oauth_flows: []
overview: Materials Project secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Materials Project
provider_slug: materials-project
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/materials-project-openapi.yml
  type: apiKey
slug: materials-project-authentication
source_filename: materials-project-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/materials-project-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/materials-project-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/materials-project/refs/heads/main/authentication/materials-project-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Chemistry
- Materials Science
- Physics
- Research
- Scientific Computing
---
