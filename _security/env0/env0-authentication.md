---
api_key_in: []
api_specs:
- filename: env0-openapi.yml
  format: yaml
  label: Env0
  slug: env0
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/openapi/env0-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Env0 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Env0 secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Env0
provider_slug: env0
scheme_count: 1
schemes:
- description: HTTP Basic Authentication. Username is the env0 API Key ID and the password is the API Key Secret, both created in the env0 organization settings.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/env0-openapi.yml
  type: http
slug: env0-authentication
source_filename: env0-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/env0-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication. Username is the env0 API Key ID and the password is\n    the API Key Secret, both created in the env0 organization settings.\n  sources:\n  - openapi/env0-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/env0/refs/heads/main/authentication/env0-authentication.yml
summary_line: http · 1 scheme
tags:
- FinOps
- Infrastructure as Code
- DevOps
- Cloud
---
