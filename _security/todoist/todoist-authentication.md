---
api_key_in: []
api_specs:
- filename: todoist-sync-api-openapi.yml
  format: yaml
  label: Todoist Sync API v9
  slug: todoist-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/todoist/refs/heads/main/openapi/todoist-sync-api-openapi.yml
- filename: todoist-comments-api-openapi.yml
  format: yaml
  label: Todoist Comments API
  slug: todoist-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/todoist/refs/heads/main/openapi/todoist-comments-api-openapi.yml
- filename: todoist-labels-api-openapi.yml
  format: yaml
  label: Todoist Labels API
  slug: todoist-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/todoist/refs/heads/main/openapi/todoist-labels-api-openapi.yml
- filename: todoist-projects-api-openapi.yml
  format: yaml
  label: Todoist Projects API
  slug: todoist-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/todoist/refs/heads/main/openapi/todoist-projects-api-openapi.yml
- filename: todoist-reminders-api-openapi.yml
  format: yaml
  label: Todoist Reminders API
  slug: todoist-reminders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/todoist/refs/heads/main/openapi/todoist-reminders-api-openapi.yml
- filename: todoist-sections-api-openapi.yml
  format: yaml
  label: Todoist Sections API
  slug: todoist-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/todoist/refs/heads/main/openapi/todoist-sections-api-openapi.yml
- filename: todoist-sync-api-openapi.yml
  format: yaml
  label: Todoist Sync API
  slug: todoist-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/todoist/refs/heads/main/openapi/todoist-sync-api-openapi.yml
- filename: todoist-tasks-api-openapi.yml
  format: yaml
  label: Todoist Tasks API
  slug: todoist-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/todoist/refs/heads/main/openapi/todoist-tasks-api-openapi.yml
- filename: todoist-user-api-openapi.yml
  format: yaml
  label: Todoist User API
  slug: todoist-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/todoist/refs/heads/main/openapi/todoist-user-api-openapi.yml
- filename: todoist-workspaces-api-openapi.yml
  format: yaml
  label: Todoist Workspaces API
  slug: todoist-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/todoist/refs/heads/main/openapi/todoist-workspaces-api-openapi.yml
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
- Task
- To-Do
- Task Management
- Collaboration
---
