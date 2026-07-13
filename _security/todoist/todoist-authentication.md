---
api_key_in: []
api_specs:
- filename: todoist-openapi.yml
  format: yaml
  label: Todoist API
  slug: todoist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/todoist/refs/heads/main/openapi/todoist-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Todoist Authentication
name_suffix: Authentication
oauth_flows: []
overview: Todoist secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Todoist
provider_slug: todoist
scheme_count: 1
schemes:
- description: Personal API token or OAuth 2.0 access token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/todoist-openapi.yml
  type: http
slug: todoist-authentication
source_filename: todoist-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/todoist-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Personal API token or OAuth 2.0 access token\n  sources:\n  - openapi/todoist-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/todoist/refs/heads/main/authentication/todoist-authentication.yml
summary_line: http · 1 scheme
tags:
- Productivity
- Tasks
- To-Do
- Task Management
- Collaboration
---
