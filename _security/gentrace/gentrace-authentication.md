---
api_key_in: []
api_specs:
- filename: gentrace-openapi-original.json
  format: json
  label: Gentrace API
  slug: gentrace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gentrace/refs/heads/main/openapi/gentrace-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gentrace Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gentrace secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gentrace
provider_slug: gentrace
scheme_count: 1
schemes:
- description: 'Enter Gentrace API key (Format: Authorization: Bearer <token>)'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/gentrace-openapi-original.json
  type: http
slug: gentrace-authentication
source_filename: gentrace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/gentrace-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Enter Gentrace API key (Format: Authorization: Bearer <token>)'\n  sources:\n  - openapi/gentrace-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gentrace/refs/heads/main/authentication/gentrace-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Ai
- LLM
- Evaluation
- Testing
- Observability
- Machine Learning
- Developer Tools
---
