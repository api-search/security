---
anonymous_access: false
api_key_in: []
api_specs:
- filename: microsoft-to-do-me-todo-api-openapi.yml
  format: yaml
  label: Microsoft To Do Me.todo API
  slug: microsoft-to-do-me-todo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-to-do/openapi/microsoft-to-do-me-todo-api-openapi.yml
- filename: microsoft-to-do-users-todo-api-openapi.yml
  format: yaml
  label: Microsoft To Do Users.todo API
  slug: microsoft-to-do-users-todo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-to-do/openapi/microsoft-to-do-users-todo-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Microsoft To Do Authentication
name_suffix: Authentication
oauth_flows: []
overview: Microsoft To Do secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Microsoft To Do
provider_slug: microsoft-to-do
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/_superseded/microsoft-to-do-checklist-items-api-openapi.yml
  - openapi/_superseded/microsoft-to-do-linkedresources-api-openapi.yml
  - openapi/_superseded/microsoft-to-do-tasklists-api-openapi.yml
  - openapi/_superseded/microsoft-to-do-tasks-api-openapi.yml
  type: http
slug: microsoft-to-do-authentication
source_filename: microsoft-to-do-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/_superseded/microsoft-to-do-checklist-items-api-openapi.yml, openapi/_superseded/microsoft-to-do-linkedresources-api-openapi.yml,\n  openapi/_superseded/microsoft-to-do-tasklists-api-openapi.yml, openapi/_superseded/microsoft-to-do-tasks-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/_superseded/microsoft-to-do-checklist-items-api-openapi.yml\n  - openapi/_superseded/microsoft-to-do-linkedresources-api-openapi.yml\n  - openapi/_superseded/microsoft-to-do-tasklists-api-openapi.yml\n  - openapi/_superseded/microsoft-to-do-tasks-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-to-do/authentication/microsoft-to-do-authentication.yml
summary_line: http · 1 scheme
tags:
- Microsoft
- Microsoft 365
- Productivity
- Task
- Task Management
- Microsoft Graph
---
