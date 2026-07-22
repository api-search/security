---
api_key_in: []
api_specs:
- filename: workflowy-api-openapi.yml
  format: yaml
  label: Workflowy API
  slug: workflowy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workflowy/refs/heads/main/openapi/workflowy-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Workflowy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Workflowy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Workflowy
provider_slug: workflowy
scheme_count: 1
schemes:
- description: Workflowy API key sent as a bearer token in the Authorization header. Generate a key at https://workflowy.com/api-key/.
  name: apiKey
  scheme: bearer
  sources:
  - openapi/workflowy-api-openapi.yml
  type: http
slug: workflowy-authentication
source_filename: workflowy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://workflowy.com/api-reference/\ndocs: https://workflowy.com/api-reference/\nkey_management: https://workflowy.com/api-key/\nnotes: >-\n  The API reference documents a single auth mechanism - a Workflowy API key\n  sent as a bearer token (\"Authorization: Bearer <YOUR_API_KEY>\"). Keys are\n  generated at https://workflowy.com/api-key/. No OAuth, no scopes.\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: Workflowy API key sent as a bearer token in the Authorization header. Generate\n    a key at https://workflowy.com/api-key/.\n  sources:\n  - openapi/workflowy-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workflowy/refs/heads/main/authentication/workflowy-authentication.yml
summary_line: http · 1 scheme
tags:
- Productivity
- Notes
- Outliner
- Task Management
- Lists
- Collaboration
- Knowledge Management
- AI Assistant
---
