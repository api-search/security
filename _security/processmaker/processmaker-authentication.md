---
api_key_in: []
api_specs:
- filename: processmaker-environment-variables-api-openapi.yml
  format: yaml
  label: ProcessMaker Environment Variables API
  slug: processmaker-environment-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/processmaker/refs/heads/main/openapi/processmaker-environment-variables-api-openapi.yml
- filename: processmaker-files-api-openapi.yml
  format: yaml
  label: ProcessMaker Files API
  slug: processmaker-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/processmaker/refs/heads/main/openapi/processmaker-files-api-openapi.yml
- filename: processmaker-groups-api-openapi.yml
  format: yaml
  label: ProcessMaker Groups API
  slug: processmaker-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/processmaker/refs/heads/main/openapi/processmaker-groups-api-openapi.yml
- filename: processmaker-notifications-api-openapi.yml
  format: yaml
  label: ProcessMaker Notifications API
  slug: processmaker-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/processmaker/refs/heads/main/openapi/processmaker-notifications-api-openapi.yml
- filename: processmaker-processes-api-openapi.yml
  format: yaml
  label: ProcessMaker Processes API
  slug: processmaker-processes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/processmaker/refs/heads/main/openapi/processmaker-processes-api-openapi.yml
- filename: processmaker-requests-api-openapi.yml
  format: yaml
  label: ProcessMaker Requests API
  slug: processmaker-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/processmaker/refs/heads/main/openapi/processmaker-requests-api-openapi.yml
- filename: processmaker-screens-api-openapi.yml
  format: yaml
  label: ProcessMaker Screens API
  slug: processmaker-screens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/processmaker/refs/heads/main/openapi/processmaker-screens-api-openapi.yml
- filename: processmaker-settings-api-openapi.yml
  format: yaml
  label: ProcessMaker Settings API
  slug: processmaker-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/processmaker/refs/heads/main/openapi/processmaker-settings-api-openapi.yml
- filename: processmaker-tasks-api-openapi.yml
  format: yaml
  label: ProcessMaker Tasks API
  slug: processmaker-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/processmaker/refs/heads/main/openapi/processmaker-tasks-api-openapi.yml
- filename: processmaker-users-api-openapi.yml
  format: yaml
  label: ProcessMaker Users API
  slug: processmaker-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/processmaker/refs/heads/main/openapi/processmaker-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Processmaker Authentication
name_suffix: Authentication
oauth_flows: []
overview: ProcessMaker secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ProcessMaker
provider_slug: processmaker
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/processmaker-platform-api-openapi.yml
  type: http
slug: processmaker-authentication
source_filename: processmaker-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/processmaker-platform-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/processmaker-platform-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/processmaker/refs/heads/main/authentication/processmaker-authentication.yml
summary_line: http · 1 scheme
tags:
- BPM
- Business Process Management
- Workflow Automation
- BPMN 2.0
- Low-Code
- Intelligent Automation
- Process Design
- Case Management
- Task Management
- Enterprise Integration
---
