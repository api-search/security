---
api_key_in:
- query
api_specs:
- filename: puma-openapi.yml
  format: yaml
  label: Puma Control/Status Application
  slug: control-app
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puma/refs/heads/main/openapi/puma-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Puma Authentication
name_suffix: Authentication
oauth_flows: []
overview: Puma secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Puma
provider_slug: puma
scheme_count: 1
schemes:
- description: Shared control-app authentication token. Configured via Puma's `--control-token` option (or `auth_token` in the control app configuration). Required on every request; missing or wrong token returns 403.
  in: query
  name: controlToken
  parameter: token
  sources:
  - openapi/puma-openapi.yml
  type: apiKey
slug: puma-authentication
source_filename: puma-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/puma-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: controlToken\n  type: apiKey\n  in: query\n  parameter: token\n  description: Shared control-app authentication token. Configured via Puma's `--control-token`\n    option (or `auth_token` in the control app configuration). Required on every request; missing\n    or wrong token returns 403.\n  sources:\n  - openapi/puma-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/puma/refs/heads/main/authentication/puma-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Web Server
- Ruby
- Rack
- Application Server
- HTTP
- Open Source
---
