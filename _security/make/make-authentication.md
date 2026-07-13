---
api_key_in:
- header
api_specs:
- filename: make-openapi.yml
  format: yaml
  label: Make API
  slug: make-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/make/refs/heads/main/openapi/make-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Make Authentication
name_suffix: Authentication
oauth_flows: []
overview: Make secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Make
provider_slug: make
scheme_count: 1
schemes:
- description: 'API token in the form: `Token <api-token>` with the required scopes enabled.'
  in: header
  name: TokenAuth
  parameter: Authorization
  sources:
  - openapi/make-openapi.yml
  type: apiKey
slug: make-authentication
source_filename: make-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/make-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: TokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API token in the form: `Token <api-token>` with the required scopes enabled.'\n  sources:\n  - openapi/make-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/make/refs/heads/main/authentication/make-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Automation
- Integration
- iPaaS
- No-Code
- Scenarios
- Workflows
---
