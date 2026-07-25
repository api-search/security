---
api_key_in:
- header
api_specs:
- filename: height-activities-api-openapi.yml
  format: yaml
  label: Height Activities API
  slug: height-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/height/refs/heads/main/openapi/height-activities-api-openapi.yml
- filename: height-field-templates-api-openapi.yml
  format: yaml
  label: Height Field Templates API
  slug: height-field-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/height/refs/heads/main/openapi/height-field-templates-api-openapi.yml
- filename: height-groups-api-openapi.yml
  format: yaml
  label: Height Groups API
  slug: height-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/height/refs/heads/main/openapi/height-groups-api-openapi.yml
- filename: height-lists-api-openapi.yml
  format: yaml
  label: Height Lists API
  slug: height-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/height/refs/heads/main/openapi/height-lists-api-openapi.yml
- filename: height-security-log-events-api-openapi.yml
  format: yaml
  label: Height Security Log Events API
  slug: height-security-log-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/height/refs/heads/main/openapi/height-security-log-events-api-openapi.yml
- filename: height-task-forms-api-openapi.yml
  format: yaml
  label: Height Task Forms API
  slug: height-task-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/height/refs/heads/main/openapi/height-task-forms-api-openapi.yml
- filename: height-tasks-api-openapi.yml
  format: yaml
  label: Height Tasks API
  slug: height-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/height/refs/heads/main/openapi/height-tasks-api-openapi.yml
- filename: height-users-api-openapi.yml
  format: yaml
  label: Height Users API
  slug: height-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/height/refs/heads/main/openapi/height-users-api-openapi.yml
- filename: height-workspace-api-openapi.yml
  format: yaml
  label: Height Workspace API
  slug: height-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/height/refs/heads/main/openapi/height-workspace-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Height Authentication
name_suffix: Authentication
oauth_flows: []
overview: Height secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Height
provider_slug: height
scheme_count: 1
schemes:
- description: "The Height API uses API keys to authenticate requests. **You can view your API key in the Height settings under API**.\n ex: `api-key secret_1234`"
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/height-height-api-openapi.yml
  type: apiKey
slug: height-authentication
source_filename: height-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/height-height-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    The Height API uses API keys to authenticate requests. **You can view your API key in the Height settings under API**.\n     ex: `api-key secret_1234`\n  sources:\n  - openapi/height-height-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/height/refs/heads/main/authentication/height-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Project Management
- Task Management
- Collaboration
- Productivity
- Workflow Automation
- AI
---
