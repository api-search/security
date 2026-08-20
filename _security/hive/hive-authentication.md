---
api_key_in:
- header
api_specs:
- filename: hive-actions-api-openapi.yml
  format: yaml
  label: Hive Actions API
  slug: hive-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hive/refs/heads/main/openapi/hive-actions-api-openapi.yml
- filename: hive-agile-sprints-api-openapi.yml
  format: yaml
  label: Hive Agile Sprints API
  slug: hive-agile-sprints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hive/refs/heads/main/openapi/hive-agile-sprints-api-openapi.yml
- filename: hive-dashboard-widgets-api-openapi.yml
  format: yaml
  label: Hive Dashboard Widgets API
  slug: hive-dashboard-widgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hive/refs/heads/main/openapi/hive-dashboard-widgets-api-openapi.yml
- filename: hive-form-submissions-api-openapi.yml
  format: yaml
  label: Hive Form Submissions API
  slug: hive-form-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hive/refs/heads/main/openapi/hive-form-submissions-api-openapi.yml
- filename: hive-messages-api-openapi.yml
  format: yaml
  label: Hive Messages API
  slug: hive-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hive/refs/heads/main/openapi/hive-messages-api-openapi.yml
- filename: hive-projects-api-openapi.yml
  format: yaml
  label: Hive Projects API
  slug: hive-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hive/refs/heads/main/openapi/hive-projects-api-openapi.yml
- filename: hive-resource-assignments-api-openapi.yml
  format: yaml
  label: Hive Resource Assignments API
  slug: hive-resource-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hive/refs/heads/main/openapi/hive-resource-assignments-api-openapi.yml
- filename: hive-teams-api-openapi.yml
  format: yaml
  label: Hive Teams API
  slug: hive-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hive/refs/heads/main/openapi/hive-teams-api-openapi.yml
- filename: hive-users-api-openapi.yml
  format: yaml
  label: Hive Users API
  slug: hive-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hive/refs/heads/main/openapi/hive-users-api-openapi.yml
- filename: hive-webhooks-api-openapi.yml
  format: yaml
  label: Hive Webhooks API
  slug: hive-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hive/refs/heads/main/openapi/hive-webhooks-api-openapi.yml
- filename: hive-workflows-api-openapi.yml
  format: yaml
  label: Hive Workflows API
  slug: hive-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hive/refs/heads/main/openapi/hive-workflows-api-openapi.yml
- filename: hive-workspaces-api-openapi.yml
  format: yaml
  label: Hive Workspaces API
  slug: hive-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hive/refs/heads/main/openapi/hive-workspaces-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Hive Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hive secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hive
provider_slug: hive
scheme_count: 1
schemes:
- description: Workspace-scoped API token issued from Hive admin settings.
  in: header
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/hive-openapi.yml
  type: apiKey
slug: hive-authentication
source_filename: hive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hive-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: api_key\n  description: Workspace-scoped API token issued from Hive admin settings.\n  sources:\n  - openapi/hive-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hive/refs/heads/main/authentication/hive-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Project Management
- Task Management
- Team Collaboration
- Productivity
- Workflow-Automation
- Time Tracking
---
