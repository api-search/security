---
api_key_in:
- header
api_specs:
- filename: robocorp-assets-api-openapi.yml
  format: yaml
  label: Robocorp Assets API
  slug: robocorp-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/robocorp/refs/heads/main/openapi/robocorp-assets-api-openapi.yml
- filename: robocorp-assistants-api-openapi.yml
  format: yaml
  label: Robocorp Assistants API
  slug: robocorp-assistants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/robocorp/refs/heads/main/openapi/robocorp-assistants-api-openapi.yml
- filename: robocorp-process-runs-api-openapi.yml
  format: yaml
  label: Robocorp Process Runs API
  slug: robocorp-process-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/robocorp/refs/heads/main/openapi/robocorp-process-runs-api-openapi.yml
- filename: robocorp-processes-api-openapi.yml
  format: yaml
  label: Robocorp Processes API
  slug: robocorp-processes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/robocorp/refs/heads/main/openapi/robocorp-processes-api-openapi.yml
- filename: robocorp-step-runs-api-openapi.yml
  format: yaml
  label: Robocorp Step Runs API
  slug: robocorp-step-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/robocorp/refs/heads/main/openapi/robocorp-step-runs-api-openapi.yml
- filename: robocorp-task-packages-api-openapi.yml
  format: yaml
  label: Robocorp Task Packages API
  slug: robocorp-task-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/robocorp/refs/heads/main/openapi/robocorp-task-packages-api-openapi.yml
- filename: robocorp-vault-api-openapi.yml
  format: yaml
  label: Robocorp Vault API
  slug: robocorp-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/robocorp/refs/heads/main/openapi/robocorp-vault-api-openapi.yml
- filename: robocorp-webhooks-api-openapi.yml
  format: yaml
  label: Robocorp Webhooks API
  slug: robocorp-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/robocorp/refs/heads/main/openapi/robocorp-webhooks-api-openapi.yml
- filename: robocorp-work-items-api-openapi.yml
  format: yaml
  label: Robocorp Work Items API
  slug: robocorp-work-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/robocorp/refs/heads/main/openapi/robocorp-work-items-api-openapi.yml
- filename: robocorp-worker-groups-api-openapi.yml
  format: yaml
  label: Robocorp Worker Groups API
  slug: robocorp-worker-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/robocorp/refs/heads/main/openapi/robocorp-worker-groups-api-openapi.yml
- filename: robocorp-workers-api-openapi.yml
  format: yaml
  label: Robocorp Workers API
  slug: robocorp-workers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/robocorp/refs/heads/main/openapi/robocorp-workers-api-openapi.yml
- filename: robocorp-workspace-api-openapi.yml
  format: yaml
  label: Robocorp Workspace API
  slug: robocorp-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/robocorp/refs/heads/main/openapi/robocorp-workspace-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Robocorp Authentication
name_suffix: Authentication
oauth_flows: []
overview: Robocorp secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Robocorp
provider_slug: robocorp
scheme_count: 1
schemes:
- description: API key with RC-WSKEY prefix (e.g., "RC-WSKEY your-api-key")
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/robocorp-control-room-openapi.yml
  type: apiKey
slug: robocorp-authentication
source_filename: robocorp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/robocorp-control-room-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key with RC-WSKEY prefix (e.g., \"RC-WSKEY your-api-key\")\n  sources:\n  - openapi/robocorp-control-room-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/robocorp/refs/heads/main/authentication/robocorp-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- RPA
- Workflow-Automation
- Python
- Open-Source
- Automation
---
