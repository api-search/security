---
api_key_in:
- header
api_specs:
- filename: openapi.json
  format: json
  label: Robocorp Control Room API
  slug: control-room-api
  spec_type: OpenAPI
  url: https://robocorp.com/api/openapi.json
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
- Workflow Automation
- Python
- Open Source
- Automation
---
