---
api_key_in:
- query
api_specs:
- filename: openapi.yml
  format: yaml
  label: Tettra REST API
  slug: tettra-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tettra/refs/heads/main/openapi/openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tettra Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tettra secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tettra
provider_slug: tettra
scheme_count: 1
schemes:
- description: API key for authentication. Available on Scaling and Enterprise plans. Determines the acting user for operations such as creating questions.
  in: query
  name: apiKey
  parameter: api_key
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: tettra-authentication
source_filename: tettra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: API key for authentication. Available on Scaling and Enterprise plans. Determines\n    the acting user for operations such as creating questions.\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tettra/refs/heads/main/authentication/tettra-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Knowledge Management
- AI
- Team Collaboration
- Wiki
- Slack Integration
- Q&A Bot
- Internal Documentation
---
