---
api_key_in: []
api_specs:
- filename: scorecard-openapi-original.yml
  format: yaml
  label: Scorecard API
  slug: scorecard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scorecard/refs/heads/main/openapi/scorecard-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Scorecard Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scorecard secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Scorecard
provider_slug: scorecard
scheme_count: 1
schemes:
- bearerFormat: starts with ak_
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/scorecard-openapi-original.yml
  type: http
slug: scorecard-authentication
source_filename: scorecard-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/scorecard-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  bearerFormat: starts with ak_\n  sources:\n  - openapi/scorecard-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scorecard/refs/heads/main/authentication/scorecard-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI
- Agents
- Evaluation
- Testing
- LLM
- Observability
- Simulation
- Developer Tools
- MCP
---
