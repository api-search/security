---
api_key_in: []
api_specs:
- filename: gitar-openapi-original.json
  format: json
  label: Gitar External API
  slug: gitar-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitar/refs/heads/main/openapi/gitar-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gitar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gitar secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gitar
provider_slug: gitar
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/gitar-openapi-original.json
  type: http
slug: gitar-authentication
source_filename: gitar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/gitar-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/gitar-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gitar/refs/heads/main/authentication/gitar-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Developer Tools
- Code Review
- CI/CD
- Code Quality
- AI
- Developer Productivity
- Automation
---
