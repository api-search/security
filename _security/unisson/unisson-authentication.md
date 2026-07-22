---
api_key_in: []
api_specs:
- filename: unisson-openapi-original.json
  format: json
  label: Unisson Platform API
  slug: unisson-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unisson/refs/heads/main/openapi/unisson-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Unisson Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unisson secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Unisson
provider_slug: unisson
scheme_count: 1
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/unisson-openapi-original.json
  type: http
slug: unisson-authentication
source_filename: unisson-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/unisson-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/unisson-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unisson/refs/heads/main/authentication/unisson-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- AI Agents
- Customer Success
- B2B Software
- Implementation
- Automation
- Agents
---
