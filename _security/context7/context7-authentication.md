---
api_key_in: []
api_specs:
- filename: context7-openapi.yml
  format: yaml
  label: Context7 REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/context7/refs/heads/main/openapi/context7-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Context7 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Context7 secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Context7
provider_slug: context7
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/context7-openapi.yml
  type: http
slug: context7-authentication
source_filename: context7-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/context7-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/context7-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/context7/refs/heads/main/authentication/context7-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Context
- Documentation
- LLM
- MCP
---
