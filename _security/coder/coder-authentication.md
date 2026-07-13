---
api_key_in:
- header
api_specs:
- filename: swagger.json
  format: json
  label: Coder REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/coder/coder/main/coderd/apidoc/swagger.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Coder Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coder secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Coder
provider_slug: coder
scheme_count: 1
schemes:
- in: header
  name: CoderSessionToken
  parameter: Coder-Session-Token
  sources:
  - openapi/coder-rest-api-openapi.yml
  type: apiKey
slug: coder-authentication
source_filename: coder-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/coder-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: CoderSessionToken\n  type: apiKey\n  in: header\n  parameter: Coder-Session-Token\n  sources:\n  - openapi/coder-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coder/refs/heads/main/authentication/coder-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Developer Tools
- Remote Development
- Cloud Development Environments
- AI Agents
- Infrastructure
- Workspaces
---
